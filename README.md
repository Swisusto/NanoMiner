# NanoMiner
Arduino Nano Miner for Duino Coin
![DuinoCoinI2C_3xNano](https://github.com/Swisusto/NanoMiner/assets/62308320/aea5d9ee-71ad-413c-aa11-4e044f7179e6)


<h3>PARTS</h3>
9 ARDUINO NANO (old or new BOOTLOADER)
1 ESP8266 WEMOS D1
WALLET IN DUINO-COIN SITE 


<h3>UPLOAD ARDUINO NANO CODE</h3>
<b>DUINOCOIN_RPI_TINY_SLAVE.INO</b>
Arduino NANO have the some code with the unique variation in the <b>I2CS_START_ADDRESS</b>
<code>
/****************** USER MODIFICATION START ****************/
#define DEV_INDEX                   0
#define I2CS_START_ADDRESS          1            <------ increment this line and upload in every NANO
#define I2CS_FIND_ADDR              true
#define WDT_EN                      false        // recommended 'true', but do not turn on if using old bootloader
#define CRC8_EN                     true
#define LED_EN                      true
#define SENSOR_EN                   true
/****************** USER MODIFICATION END ******************/
</code>

<h3>UPLOAD ARDUINO ESP8266 CODE</h3>
Modify this file with your, wifi, duino-coin credentials etc
<code>
const char* ssid          = "WIFI_NAME";         // Change this to your WiFi SSID
const char* password      = "PASSWORD";         // Change this to your WiFi password
const char* ducouser      = "DUCO_USER";  // Change this to your Duino-Coin username
const char* rigIdentifier = "RIG_ID";  // Change this if you want a custom miner name
const char* mDNSRigIdentifier = "esp";  // Change this if you want a custom local mDNS miner name
String mining_key         = "MINERKEY";     // Change this if wallet is protected with mining key
</code>
<br>

HAPPY MINING!!
<br>
For more info contact me or follow me on my patreon for more projects
<br>
<a href="https://www.patreon.com/LASERandCNC">FOLLOW ME ON PATREON



