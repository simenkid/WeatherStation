[TODO]
1. Overview detail descriptions
2. Pinouts detail descriptions
3. Assembly module Picture & descriptions
4. How to use BLE shepherd(freebird) detail descriptions
5. Electrical Specifications test value
6. upload Schematic picture




# WeatherStation
---  
![WeatherStation ](http://imgur.com/blQHcna "WeatherStation ")  

## Guide Content  

1. [Overiew](#Overiew)  
2. [Pinouts](#Pinouts)  
3. [Assembly](#Assembly)  
4. [How to use](#How to use)  
5. [Electrical Specifications](#Electrical Specifications)  
6. [Downloads](#Downloads)  


<a name="Overiew"></a>
## 1. Overview  

This module have 4 functions, it can measure pressure, UV, voice dB value, temperature and humidity. Most sensors is . Ex: control light on/off, to send a message, etc. Buttons's function are assigned by programmer and this functions will be transmit by BLE module.  

* Features
  * Measure temperature & humidity with SHT20
  * Measure ambient light/UVI with Si1132
  * Measure sound level with on-board Mic
    Range:30 to 80dB
  * Measure air pressure level with LPS25HB
    Range:260hPa to 1260hPa
    Altitude: 10100m to -1875m
    Resolution: 0.03 hPa (0.25m)
  * Connect a DSM501A dust sensor to measure PM2.5/PM10 (optional)

<a name="Pinouts"></a>
## 2. Pinouts  

* Power Pins:  
  * Vcc  
  * GND  
* I2C  
  * SDA  
  * SCL  
* PM2.5
  * Vo1
  * Vo1
* P_INT
* MIC

<a name="Assembly"></a>
## 3. Assembly  

#### USB 5V Power module  
#### BLE module  
#### WeatherStation module  

<a name="How to use"></a>
## 4. How to use  

* BLE Dongle + BLE shepherd(freebird)  
* How to use BLE shepherd(freebird)  

<a name="Electrical Specifications"></a>
## 5. Electrical Specifications   

| Parameter         | Absolute Maximum Rating  | Uints  
|-------------------|--------------------------|-------------  
| Power             |                          |  W  
| Operating current |                          |  A  
| Vcc to Gound      |                          |  V  
| 5V to Ground      |                          |  V  

<a name="Downloads"></a>
## 6. Downloads  

[LM358 Datasheets](http://www.ti.com/lit/ds/symlink/lm358.pdf "LM358")  
[Si1132 Datasheets](https://www.silabs.com/Support%20Documents/TechnicalDocs/Si1132.pdf "Si1132")  
[SHT20 Datasheets](https://www.sensirion.com/fileadmin/user_upload/customers/sensirion/Dokumente/Humidity_Sensors/Sensirion_Humidity_Sensors_SHT20_Datasheet_V4.pdf "SHT20")  
[SPW2430HR5H-B Datasheets](http://www.mouser.com/ds/2/218/-531228.pdf "SPW2430HR5H-B")  
[LPS25HB Datasheets](http://www.st.com/content/ccc/resource/technical/document/datasheet/9a/4c/aa/72/1f/45/4e/24/DM00141379.pdf/files/DM00141379.pdf/jcr:content/translations/en.DM00141379.pdf "LPS25HB")  

Schematic  

