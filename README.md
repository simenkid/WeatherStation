# WeatherStation  
---  

## Guide Content  

1. [Introduction](#Introduction)  
2. [Hardware Overview](#Hardware Overview)  
3. [Usage](#Usage)  
4. [Reference](#Reference)  


<a name="Introduction"></a>
## 1. Introduction  

Sivann的WeatherStation模組有光度、壓力、溫度、濕度、聲音以及空氣的塵埃 (選擇性，需自己購買 PM 2.5/PM10加裝) 的感測器。模組上的光度感測器 (Si1132) 可量測紫外線 (UV) 、環境光 (Ambient light)，壓力感測器 (LPS25HB) 可量測大氣壓力，而溫溼度感測器 (SHT20) 量測溫溼度而麥克風 (SPW2430HR5H) 量測聲音的響度，其相關的詳細資料在Reference，請自行參閱。  

#### Sivann模組疊合  
Sivann 有感測模組外、無線模組以及電源模組，使用者可以將模組疊合使用，相關介紹在 sivann 模組疊合介紹。  

* Features  
  * 量測紫外線指標 (UVI)以及環境光 (Ambient light)。  
  * 量測大氣壓力。  
  * 量測溫度、溼度。  
  * 量測聲音的變化。  
  * 量測空氣塵埃(選擇性)。  

<a name="Hardware Overview"></a>
## 2. Hardware Overview  

![WeatherStation](http://i.imgur.com/5QK3wNmm.png "WeatherStation")

### Pinouts  
* Power Pins:  
  * 5V – 5V的電源腳位。供電給 LM358 及 PM2.5/PM10 (選擇性)。  
  * Vcc (3.3V) – 3.3V 的電源腳位。供電給 SPW2430HR5H。  
  * Vdd (3.3V) – 3.3V 的電源腳位。供電給 LPS25HB、Si1132 以及 SHT20。
  * GND – 5V、Vcc 及 Vdd 共同的地。   
* I2C Pins 
  * SDA – I2C 的資料腳位。 
  * SCL – I2C 的時脈腳位。 
* P_INT
LPS25HB 的中斷，發生中斷的情況設定請參閱 Reference 的 LPS25HB。
* UV_INT
Si1132 的中斷，發生中斷的情況設定請參閱 Reference 的 Si1132。
* MIC 
麥克風 (SPW2430HR5H) 的電壓輸出。
* PM2.5 (選擇性)
  * Vo1
  * Vo2

<a name="Usage"></a>
## 3. Usage  

1.	連接5V、Vdd (3.3V) 及Vcc (3.3V) 至電源供應。
2.	連接 GND 至電源供應的地。
3.	連接 I2C (SDA, SCL) 至微控制器的 I2C 腳位。
4.	在 I2C (SDA, SCL) 連接上拉電阻 (如果使用 sivann 模組疊合則不須接)，推薦值 5k~1k 歐姆 (一般模式~快速模式)。
5.	連接 MIC 至微控制器的 ADC 輸入腳位。
6.	連接 UV_INT、P_INT 至微控制器的輸入腳位。

<a name="Reference"></a>
## 4. Reference   

[LM358 Datasheets](http://www.ti.com/lit/ds/symlink/lm358.pdf "LM358")  
[Si1132 Datasheets](https://www.silabs.com/Support%20Documents/TechnicalDocs/Si1132.pdf "Si1132")  
[SHT20 Datasheets](https://www.sensirion.com/fileadmin/user_upload/customers/sensirion/Dokumente/Humidity_Sensors/Sensirion_Humidity_Sensors_SHT20_Datasheet_V4.pdf "SHT20")  
[SPW2430HR5H-B Datasheets](http://www.mouser.com/ds/2/218/-531228.pdf "SPW2430HR5H-B")  
[LPS25HB Datasheets](http://www.st.com/content/ccc/resource/technical/document/datasheet/9a/4c/aa/72/1f/45/4e/24/DM00141379.pdf/files/DM00141379.pdf/jcr:content/translations/en.DM00141379.pdf "LPS25HB")  

Schematic  

