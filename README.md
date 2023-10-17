# LogBogRobotter

# CarWIFI 

Materialer:

NodeMCU (ESP8266)
ESP12E motor shield
TT-motor
8 AA batterier
Ledninger

Kode:

Vi inkluderede "ESP8266WiFi" biblioteket for at give NodeMCU'en mulighed for at oprette forbindelse til et trådløst netværk ved hjælp af SSID og adgangskode.
Vi brugte også "ESP8266WebServer" biblioteket til at oprette en HTTP-server, der kunne modtage kommandoer via Wi-Fi til styring af motoren.

Beskrivelse:

Vores projekt involverede oprettelse af en Wi-Fi-styret bil ved hjælp af NodeMCU og en TT-motor for at opnå dette brugte vi en ESP12E motor shield og forsynede den med strøm fra 8 AA-batterier
NodeMCU'en blev konfigureret til at oprette forbindelse til et eksisterende trådløst netværk ved hjælp af SSID og adgangskode så vi kunne styre bilen via Wi-Fi
En HTTP-server blev oprettet på NodeMCU'en ved hjælp af ESP8266WebServer-biblioteket denne server kunne modtage kommandoer fra en fjernenhed som vi kunne bruge til at styre motorens retning og hastighed

3D-Model:

Udover at arbejde med hardware og kode oprettede vi også en brugerdefineret 3D-model af en bil der blev brugt som en del af vores projekt denne model blev skabt i henhold til vores egne design

![370207219_1426954907879265_2228441281571694687_n](https://github.com/ArsimBoy420/LogBogRobotter/assets/113034331/78adb7fb-dda8-4418-8f50-8b142fc3b490)
![image](https://github.com/ArsimBoy420/LogBogRobotter/assets/113034331/016a9bd4-7338-45e4-9784-3f7825a5dba4)
![image](https://github.com/ArsimBoy420/LogBogRobotter/assets/113034331/2fd59a0d-ea55-4914-9a8e-4ad6a8885548)

Ideer som vi havde:


![image](https://github.com/ArsimBoy420/LogBogRobotter/assets/113034331/f1b383aa-2cac-456c-9b32-72654bd6200c)
![image](https://github.com/ArsimBoy420/LogBogRobotter/assets/113034331/f1fca3cb-e145-4318-a2f6-a3d231d25e88)


Her er en video hvordan den virker med WIFI:

https://github.com/ArsimBoy420/LogBogRobotter/assets/113034331/bb4669db-72ee-4560-bce9-da2593f6ac08



# 25-08-2023 Trafiklys

I dag fik vi opgave til at lave et trafiklys med 8 state(8s) hvor vi fik noget redskaber som man kan se på billede her:
![20230830_194850](https://github.com/ArsimBoy420/LogBogRobotter/assets/113034331/96116ca2-98bb-45e9-8ecb-1233aaa9eb84)

https://github.com/ArsimBoy420/LogBogRobotter/assets/113034331/96bfe68f-a195-445a-b0ef-d51295782069


Jeg blev færdig med trafiklyset hvor den køre igennem de 8 state med 6 lys jeg har så brugt switch hvor jeg har gået ignnem 11 case


# 29-08-2023 SG90 180 grader (Tower)

I dag fik vi nogle forskellelige opgaver og min gruppe fik en SG90 som der kan dreje 180 grader rundt og en B10K som vi skulle bruge til at dreje den så vi kunne dreje SG90 vi skulle så lave en kode der ville give komandorer så vi kunne dreje på B10K her på billede her under kan man se vores slut projekt på den med den kode vi havde brugt og en lille forklaring hvordan vi har sat ledninger på:

1. Forbind NodeMCU ESP8266:
Forbind 3.3V-pinden på NodeMCU til en strømforsyning på breadboardet (f.eks. den øverste strimmel).
Forbind GND-pinden på NodeMCU til en jordforbindelse på breadboardet (f.eks. den nederste strimmel).

2. Forbind B10K Potentiometer:
Potentiometeret har 3 ben - ben 1, ben 2 og ben 3.
Forbind ben 1 på potentiometeret til strømforsyningen (f.eks. en strimmel tilsluttet 3.3V).
Forbind ben 2 på potentiometeret til en analog indgangspin på NodeMCU (f.eks. A0).
Forbind ben 3 på potentiometeret til jordforbindelsen (f.eks. en strimmel tilsluttet GND).

3. Forbind SG90 Servo:
Forbind den røde ledning (strøm) på SG90 til strømforsyningen (f.eks. en strimmel tilsluttet 3.3V).
Forbind den brune ledning (jord) på SG90 til jordforbindelsen (f.eks. en strimmel tilsluttet GND).
Forbind den orange ledning (signal) på SG90 til en digital pin på NodeMCU (f.eks. D1).

![20230829_205542](https://github.com/ArsimBoy420/LogBogRobotter/assets/113034331/3c2f972e-7e79-4e97-a8b5-9db16f412bad)
![20230829_205549](https://github.com/ArsimBoy420/LogBogRobotter/assets/113034331/f788bc49-3128-4b34-9a80-0fb4f33d18e6)

https://github.com/ArsimBoy420/LogBogRobotter/assets/113034331/13c1be1a-3f4d-41bb-8758-eb5da35d4ae3
