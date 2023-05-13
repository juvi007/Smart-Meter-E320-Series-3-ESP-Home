# Smart-Meter-E320-Series-3-ESP-Home
Dokumentation für das Auslesen von Landis+Gyr E320 Series 3 Smart Meeter. 
 Es handelt sich um die Smart Meter die die EAM in Hessen verbaut
 
Das Smart Meter hatt für die Schnitstelle 2 Modi, die Version hier funktioniert nur bei der Erweiterten Scnitstelle, für die Aktivirung die Anleitung des Hestellers nutzen.

Hardware:
  - ESP 8266
  - ttl ir lesekopf lese-schreib-Kopf EHZ Volkszähler Hichi Smartmeter
  - Netzteil 5V und Kabel

Das Samart Meter gibt 5 obis Codes aus:
 - 1-0:96.50.1*1 & 1-0:96.1.0*255 sind Informationen über das Smart Meter
 - 1-0:1.8.0*255 Bezug aus dem Netz
 - 1-0:2.8.0*255 Einspeisung aus dem Netz
 - 1-0:16.7.0*255 Aktuelle Leistung

Bezug & Einspeißung werden in Kwh und mit 5 Nachkommastellen angeben
Die Leistung wird in W ohne Nachkomma Stellen angeben
