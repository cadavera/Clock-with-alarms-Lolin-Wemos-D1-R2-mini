Hi there lol

If you are reading this, it means you're interested in my work (and I'm really happy about it).


IMPORTANT:
You can find the connections and more information about what I used in the other files.
You will see some words in spanish into the code, im not gonna change it bc it doesnt affect the functionality lol..

BTW in the code u Will find the WIFI section, You have to put your wifi name and password so the clocl Will connect to internet
AND the USB C is conencted to the opposite side bc i used another USB wich used the oposite conection betwen 5V and GND



Description and info of the Project:

The main objective of this project was to develop an autonomous digital clock with an alarm system that can be modified from a web interface, is automatic, and is also capable of controlling 230V alarm devices.



The system consists of:
-A Wemos D1 R2 microcontroller as the central unit.

-DS1307 RTC to maintain the time.

-16x2 LCD screen for local display.

-Buzzer for audible alerts.

-Power supply via 5V USB.




General Operation:

1. Upon powering on the device:

○ The LCD screen, RTC, and Wi-Fi are initialized.

○ An attempt is made to synchronize the time using NTP (pool.ntp.org).

○ The alarms stored in the EEPROM are loaded.


2. During normal operation:

○ The screen displays the current time and the next alarm.

○ Every second, the system checks if any alarms are present.

○ The web server is active and responds to requests from web browsers. 


3. Alarm Management:

○ Alarms are stored in EEPROM (and are not lost upon reboot).

○ Alarms can be added, modified, or deleted from the web interface.

○ Supports the selection of specific days (e.g., MWTJV).

○ Maintains an order of alarms based on which is next.
