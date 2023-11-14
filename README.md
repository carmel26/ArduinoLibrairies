# Arduino Librairies for ESP3D
for ESP3D using ESP8266 board </br>
## Using Arduino 1.8.9 

***After downloading esp3d libraire from <a href="https://github.com/luc-github/ESP3D/">download version 2.1.1</a> or use the provided one in this repository</br>

*Unzip the provided librairie for ESP3D or just download a new one </br>

## for the Board use ESP8266 Dev Mod and settings as shown on the attachement image.

## if the file index.html.gz is missing 
click on upload file </br>
select the file indext.html from *** ESP3d-2.1.1/esp3d/data/index.html.gz </br>
and click on uplad and refresh the page</br>
## if you get these error :
1)correct the first error by replacing this: </br>
#include  <hwcrypto/sha.h> </br>
with this librairie  </br>
#include <esp32/sha.h> </br>
2)correct the second error by replacing this: </br>
_esp_wifi_set_config(*ESP_IF_WIFI_STA*, &wifi_config);_ </br>
with this: </br>
_esp_wifi_set_config(*WIFI_IF_STA*, &wifi_config);_ </br>
Means every where where there is ESP_IF_WIFI_STA* in the file replace it with *WIFI_IF_STA* from the source <a href="https://github.com/FujiNetWIFI/fujinet-platformio/commit/622f0e4d3a48f0d68f0c3090da6e377b36007e75" >click here</a> </br>
