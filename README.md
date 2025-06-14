# SHFW Po Polsku
SHFW Po polsku to poradnik jak zainstalować oprogramowanie SHFW (Scooter Hacking Firmware) oraz jak zrobić downgrade wersji BLE używając programatora STM8 i STM32 ST-Link V2.

# Co potrzebuje? 
Do zainstalowania SHFW potrzebujesz aplikacji Scooter Hacking Utility, którą możesz pobrac na Google Play lub plik APK na stronie https://utility.cfw.sh/ 

![image](https://github.com/user-attachments/assets/04f3ede9-b9f4-4522-95dc-113751e54437)
* gdy jesteś na stronie, klikasz download apk. i instalujesz aplikacje *
  
# Upewnij się, że twoja wersja BLE nie przekracza 1.5.5 
Jeżeli twoja wersja BLE jest wyższa niż 1.5.5, lub na ekranie pokazuje się "Restricted BLE Firmware Detected" Musisz zrobić downgrade BLE ST-Linkiem V2
Wszelakie informacje oraz poradnik znajdziesz na tym filmie: https://www.youtube.com/watch?v=IvQ4oT2u_vg

#  Jak zainstalować shfw? 
Gdy się upewniłeś, że twoja wersja BLE jest niższa niz 1.5.5, możesz zacząć flashować oprogramowanie SHFW. 
![image](https://github.com/user-attachments/assets/91ea4823-4434-4606-9a05-0a4315dbe7c7)
Przechodzisz do zakładki "FLASH", i klikasz "Install/Update SHFW".
![image](https://github.com/user-attachments/assets/11525206-18e6-4f2c-920e-5a9a69747472)
Po kliknięciu "install/update SHFW", klikasz w tą wersje, ktorą chcesz pobrać. Na czas publikacji tego poradnika znajduje się jedna wersja SHFW, co widać na zdjęciu.
Teraz zacznie się proces flashowania, POD ŻADNYM POZOREM, NIE WYŁACZAJ HULAJNOGI I MIEJ SWÓJ TELEFON BLISKO HULANOGI !!! 

Jeżeli flashowanie się zakończyło. Witaj w SHFW! 
Teraz możesz przejść do zakładki CONFIG . 

![image](https://github.com/user-attachments/assets/d31f3814-67c9-409e-a2d1-70c1085610d4)

Po flashowaniu, hulajnoga nie będzie mogla się ruszyć, bo musisz ustawic wartości. 

Możesz użyc tych, co podałem na dole:



#### $${\color{red}Xiaomi Mi Pro 2 }$$
-Throttle
Tryb Sport, Speed-based
Power limit 20-25A 
Current smoothness 800mA 
Acceleration Boost 100%


-Brake
| Build Curve | 
30A, Full quadratic. 

włączamy Motor PWM Overmodulation dla sportu

W zakładce Field Weakening, wlaczamy dla trybu sport.
20 kmh, 0A 

Variable Field current


wiecej zasięgu: 800mA


na normalną jazdę: 1200mA


na wyprzedzanie motusów: 1500mA 

W motor settings ustawiamy Motor PWM frequency na 20kHz.




#### $${\color{red}Xiaomi Essential, Lite, 1S}$$ 
Sport mode, DPC, 18A, fully quadratic (1.0).
Acceleration boost  50%.
Brake 30A, flat (0.0), jeżeli twój hamulec jest za słaby, podkręć brake boost setting. 
Motor PWM Overmodulation włączony na sport.

Field Weakening

Włączamy dla Sport. 

15 km/h, 0A, 1500.

W motor settings ustawiamy PWM Frequency na 20 kHz



#### $${\color{red}Ninebot EsX, Ex}$$ 
Sport mode, DPC, 18A, fully quadratic (1.0).
Acceleration boost, 50%.
Brake, 55A flat (0.0)
Overmodulation dla sportu 


Field Weakening
15 km/h, 0A, 1500.
