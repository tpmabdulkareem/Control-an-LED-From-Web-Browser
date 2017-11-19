# TURN ON/OFF LED USING IOT 

## Simply, a through a webpage we can turn ON or OFF the LED.

### Materials Required to do this Project.
#### 1.ESP8266 Node MCU
#### 2. Breadboard
#### 3. Wires
#### 4. LED
#### 5. Arduino IDE

Firstly open the Arduino IDE

Go to files and click on the preference in the Arduino IDE


![alt text](http://1.bp.blogspot.com/-OV1A_EMzm00/VnPsxvqxr_I/AAAAAAAAAuI/qlswMsf3Reo/s1600/preference.PNG)

copy the below code in the Additional boards Manager

http://arduino.esp8266.com/stable/package_esp8266com_index.json

click OK to close the preference Tab.


![alt text](http://1.bp.blogspot.com/-u-opNqS4BiI/VnPuR5Pc5uI/AAAAAAAAAuU/wGg5PkYGE3M/s1600/board%2Bmanager.png)



After completing the above steps , go to Tools and board, and then select board Manager


![alt text](http://1.bp.blogspot.com/-njmbyb_yr_U/VnPuv7WAjRI/AAAAAAAAAus/nj0gR7SyFuE/s1600/board%2Bmanager%2Bopen.PNG)

Navigate to esp8266 by esp8266 community and install the software for Arduino.

Once all the above process been completed we are read to program our esp8266 with Arduino IDE.


![alt text](http://3.bp.blogspot.com/-qYY0XGJiYFo/VnPwPEkNq9I/AAAAAAAAAu4/NPbST-BezFY/s1600/blink_bb.jpg)



For this example I have used NodeMCU esp8266 and if you are using any other vendor wifi chips or generic wifi module please check with the esp8266 Pin mapping which is very essential to make things works.

The reason why I used D7 pin for this example is , I uploaded the basic blink program that comes with the examples program in the arduino IDE which is connected with 13 pin of arduino. The 13th pin is mapped into D7 pin of NodeMCU.

go to board and select the type of esp8266 you are using. and select the correct COM port to run the program on your esp8266 device.


void setup() {<br>  // initialize digital pin 13 as an output.

  pinMode(13, OUTPUT);
  
}</p><p>// the loop function runs over and over again forever
  
void loop() {

  digitalWrite(13, HIGH);   // turn the LED on (HIGH is the voltage level)
  
  delay(1000);              // wait for a second
  
  digitalWrite(13, LOW);    // turn the LED off by making the voltage LOW
  
  delay(1000);              // wait for a second
  
}
