# WeatherStation  
---  

## Guide Content  

1. [Introduction](#Introduction)  
2. [Hardware Overview](#Hardware Overview)  
3. [Usage](#Usage)  
4. [Reference](#Reference)  


<a name="Introduction"></a>
## 1. Introduction  

Sivann的WeatherStation模組可偵測光、大氣壓力、溫度、濕度、聲音以及空氣的塵埃(選擇性)。  
Si1132可感測UV、IR以及可見光，LPS25HB感測大氣壓力，SHT20感測溫度、溼度，SPW2430HR5H感測聲音，其相關的詳細資料在Reference，請自行參閱。  
#### Sivann模組疊合  
Sivann除了感測模組外還有供電模組及無線模組，使用者可以將模組疊合使用，更為方便，相關介紹在sivann模組疊合介紹。  

* Features  
  * 量測可見光、UVI以及IR  
  * 量測大氣壓力  
  * 量測溫度、溼度  
  * 量測聲音的變化  
  * 量測空氣塵埃(選擇性)  

<a name="Hardware Overview"></a>
## 2. Hardware Overview  

![WeatherStation](http://i.imgur.com/5QK3wNm.png "WeatherStation")

### Pinouts  
* Power Pins:  
  * 5V – 供電給LM358及PM2.5/PM10(選擇性)。  
  * Vcc(3.3V) – 供電給Buzzer。  
  * GND – 5V及Vcc共同的地。   
* AO  
MQ-2的電壓輸出。  
* Alarm_EN  
用來控制Buzzer。  

<a name="Usage"></a>
## 3. Usage  

供電5V及Vcc並接好GND。  

<a name="Reference"></a>
## 4. Reference   

[LM358 Datasheets](http://www.ti.com/lit/ds/symlink/lm358.pdf "LM358")  
[Si1132 Datasheets](https://www.silabs.com/Support%20Documents/TechnicalDocs/Si1132.pdf "Si1132")  
[SHT20 Datasheets](https://www.sensirion.com/fileadmin/user_upload/customers/sensirion/Dokumente/Humidity_Sensors/Sensirion_Humidity_Sensors_SHT20_Datasheet_V4.pdf "SHT20")  
[SPW2430HR5H-B Datasheets](http://www.mouser.com/ds/2/218/-531228.pdf "SPW2430HR5H-B")  
[LPS25HB Datasheets](http://www.st.com/content/ccc/resource/technical/document/datasheet/9a/4c/aa/72/1f/45/4e/24/DM00141379.pdf/files/DM00141379.pdf/jcr:content/translations/en.DM00141379.pdf "LPS25HB")  

Schematic  

