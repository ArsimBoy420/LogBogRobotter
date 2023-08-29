# LogBogRobotter

25-08-2023
Trafiklys


I dag fik vi opgave til at lave et trafiklys med 8 state(8s) hvor vi fik noget redskaber som man kan se på billede her:



29-08-2023 
SG90 180 grader

I dag fik vi nogle forskellelige opgaver og min gruppe fik en SG90 som der kan dreje 180 grader rundt og en B10K som vi skulle bruge til at dreje den så vi kunne dreje SG90 vi skulle så lave en kode der ville give komandorer så vi kunne dreje på B10K her på billede her under kan man se vores slut projekt på den med den kode vi havde brugt:

og en lille forklaring hvordan vi har sat ledninger på:

1. Forbind NodeMCU ESP8266:
Forbind 3.3V-pinden på NodeMCU til en strømforsyning på breadboardet (f.eks. den øverste strimmel).
Forbind GND-pinden på NodeMCU til en jordforbindelse på breadboardet (f.eks. den nederste strimmel).

2. Forbind B10K Potentiometer:
Potentiometeret har 3 ben - ben 1, ben 2 og ben 3.
Forbind ben 1 på potentiometeret til strømforsyningen (f.eks. en strimmel tilsluttet 3.3V).
Forbind ben 2 på potentiometeret til en analog indgangspin på NodeMCU (f.eks. A0).
Forbind ben 3 på potentiometeret til jordforbindelsen (f.eks. en strimmel tilsluttet GND).

3.Forbind SG90 Servo:
Forbind den røde ledning (strøm) på SG90 til strømforsyningen (f.eks. en strimmel tilsluttet 3.3V).
Forbind den brune ledning (jord) på SG90 til jordforbindelsen (f.eks. en strimmel tilsluttet GND).
Forbind den orange ledning (signal) på SG90 til en digital pin på NodeMCU (f.eks. D1).

![20230829_205542](https://github.com/ArsimBoy420/LogBogRobotter/assets/113034331/3c2f972e-7e79-4e97-a8b5-9db16f412bad)
![20230829_205549](https://github.com/ArsimBoy420/LogBogRobotter/assets/113034331/f788bc49-3128-4b34-9a80-0fb4f33d18e6)

Koden: 

#include <Servo.h> 
#include <Arduino.h>

Servo myservo; 
int val;

void setup()
{
  myservo.attach(D1);
}

void loop() 
{ 
  val = analogRead(A0);           
  val = map(val, 0, 1023, 0, 180);    
  myservo.write(val);                  
  delay(15);                          
} 


