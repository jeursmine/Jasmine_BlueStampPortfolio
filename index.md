# Smart Lamp
The IoT Smart Lamp is a WiFi-connected LED system that responds to motion, temperature, and user commands from anywhere in the world via Adafruit IO. One of the biggest challenges was integrating multiple sensors (motion, temperature, LDR) and syncing them with cloud-based control, but the result is a responsive, customizable light that blends automation with real-time input from the user. Completing this project was a rewarding dive into IoT, where coding, electronics, and creativity all came together.


| Jasmine Q | Homestead High School | (area of interest) | Incoming Junior |


![Headstone Image](smallestpicture.png)
  
# Final Milestone



# Second Milestone

For my second milestone, I successfully integrated all components of my smart lamp into a unified system that delivers full functionality. I also connected the project to Adafruit IO, a cloud-based platform for data communication and IoT device control. Using Adafruit IO, I created multiple data feeds to send and receive information between the lamp and the user interface on the Adafruit dashboard.My code was designed to both update these feeds with real-time sensor data and respond to user inputs—such as button presses and toggle switches—on the dashboard. This enabled seamless two-way interaction: users can remotely control the smart lamp and receive live system feedback via the dashboard.

Key features implemented include:

    -Safe Mode: When toggled on via the dashboard, this mode triggers an email alert and activates a buzzer alarm if motion is detected in the room.

    -Multicolor LED Ring: Users can select any desired color for the LED ring through the dashboard.

    -Temperature and Humidity Monitoring: The system displays real-time temperature and humidity data and sends email notifications if values go above or below specified thresholds.

    -Master Light Switch: When off, all lights are disabled. When on, the lamp will automatically turn on if motion is detected and remain on until the switch is turned off.

One major challenge I encountered was inconsistent readings from the temperature and humidity sensor—it would occasionally return extreme or invalid values (e.g., negatives or values in the millions). To solve this, I implemented a filtering system using a while loop that rejects unrealistic values and only accepts valid sensor readings. I also added a short delay before the initial reading to allow the sensor time to calibrate properly.

Next, I plan to add more features (still to be determined) and begin designing and building the enclosure for the smart lamp. I may also consider removing the motion-sensing feature from the LED light, depending on further testing and feedback.

# First Milestone

<iframe width="560" height="315" src="https://www.youtube.com/embed/_4Cy8AbWqvQ?si=k65Cnbasy8dO3p2p" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

For my first milestone, I essentially tested all sensors and components on my breadboard individually before wiring them all up onto the circuit. 

My IoT Smart Lamp integrates several sensors and components, including the DHT11 (temperature/humidity sensor), HC-SR501 (motion detector), photoresistor (light sensor), a NeoPixel 12-LED ring, and an ESP8266 microcontroller.

The project mainly relies on the ESP8266, a Wi-Fi-enabled microcontroller that allows all connected components to send and receive data over the internet. The DHT11 sensor measures both temperature and humidity. It uses a humidity sensor (which detects changes in capacitance) and a thermistor (which detects temperature changes via resistance). These readings are processed internally and output as digital data. The HC-SR501 motion sensor uses infrared to detect motion by sensing heat changes in its surroundings, signaling when movement is detected. The NeoPixel ring consists of 12 individually addressable RGB LEDs, each with its own integrated circuit. This allows for custom color and brightness control, adding a visual and aesthetic element to the lamp. Lastly, the photoresistor (or light-dependent resistor) adjusts brightness based on ambient light levels by varying its resistance depending on light exposure.

Together, these components provide a functional and customizable smart lamp system:

    -The DHT11 allows the user to monitor room temperature and humidity.
       
    -The HC-SR501 enables motion detection and potential intruder alerts.
         
    -The NeoPixel ring offers customizable ambient lighting.
    
    -The photoresistor automatically adjusts brightness based on room lighting conditions.

One of the biggest challenges I faced was that the tutorial I was originally provided used the Cayenne IoT platform, which has since shut down. This required me to search for alternative resources and experiment independently to determine the best way to wire my circuit and test individual components. Additionally, as someone with limited prior experience in physical computing and circuit wiring, I encountered some trial-and-error issues during setup. However, in the end, I was able to get the circuit functioning correctly.

In the next milestone, I will focus on uploading and integrating all the code needed to make the components work together. I will also create an Adafruit IO dashboard, allowing the user to:

    -View real-time temperature, humidity, motion, and brightness data
  
    -Customize the color of the lamp through the NeoPixel ring
  
    -Receive automated email alerts for abnormal temperature/humidity levels
  
    -Be notified when motion is detected while the lamp is in “safe mode”
  
By the end of the next milestone, the smart lamp will be fully functional, customizable, and interactive through a clean, user-friendly IoT interface.

# Schematics 

# Code

# Starter Project- Retro Arcade Console
<iframe width="560" height="315" src="https://www.youtube.com/embed/hvmn-ZRGc-s?si=3SyQsaWPOCVCY1et" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
Components: 1 buzzer, 1 electric capacitator, 1 micro USB, 1 power cable, 1 self-switch, 1 self-switch cap, 1digitron display, 1IC chip, 2 LED dot matrix modules, 6 buttons, 6 button caps, 1 PCB, 8 M3x5mm screws, 2 M3x8mm screws, 4 copper columns, 4 hexagonal columns, 1 AAA battery case, and 6 arcrylis shells.

How it works: The retro arcade console is a beginner-friendly DIY electronics project. It includes a pre-designed printed circuit board (PCB) and various electronic components like LEDs, resistors, and buttons. Users solder the components onto the PCB following clear instructions. Once assembled and powered, the kit functions as a mini interactive arcade display where the user can play various different retro arcade games such as Tetris and Snake. It's designed to help beginners practice soldering while creating a fun, working gadget.

Button Functions: 

![button image](buttoncontrols.png)

Challenges: The retro arcade console was relatively easy to assemble. The soldering was simple and was just slightly tedious due to the number of joints that needed to be made. The main challenge for me was figuring out how to connect the battery back to the PCB, given unclear instructions. Other than that, no challenges were faced. 

# Bill of Materials(Intensive Project)

| **Part** | **Note** | **Price** | **Link** |
|:--:|:--:|:--:|:--:|
| NODEMCU ESP8266 | Microcontroller Board with Wifi | $7.99	 | <a href="https://www.amazon.com/dp/B010O1G1ES/ref=twister_B086QGXBRW?_encoding=UTF8&psc=1"> Link </a> |
| DHT11	 | Temperature and Humidity Sensor | $9.99 | <a href="https://www.amazon.com/Adafruit-temperature-humidity-sensor-extras-ADA386/dp/B00NAY22V8"> Link </a> |
| NeoPixel Ring (12 LEDs) | Colorful Light with RGB | $11.40 | <a href="https://www.amazon.com/Adafruit-NeoPixel-Ring-Integrated-Drivers/dp/B00KAE3R1U/ref=sr_1_1crid=B5L3C9ZLNEGO&keywords=adafruit+neopixel+12+led&qid=1689178366&sprefix=adafruit+neopixel+12+led%2Caps%2C151&sr=8-1"> Link </a> |
| PIR Sensor | Motion Sensor | $11.99	 | <a href="(https://www.amazon.com/Adafruit-LK-918O-SANV-FBACA-PIR-Motion-Sensor/dp/B00JOZTAC6)"> Link </a> |
| LDR Sensor | Light Sensor | $7.99	 | <a href="https://www.amazon.com/BOJACK-Photoresistance-Sensitive-Resistor-GM5539/dp/B07TQMJ212/ref=sr_1_3?crid=30NPCKYPA4HL4&keywords=ldr+sensor&qid=1689181779&sprefix=ldr+sensor+adafruit%2Caps%2C184&sr=8-3"> Link </a> |
| Buzzer | Sends High Low Signals | $6.98	 | <a href="https://www.amazon.com/Cylewet-Electronic-Magnetic-Continuous-Arduino/dp/B01N7NHSY6/ref=sr_1_3?crid=WN57I7A8ZBMC&keywords=buzzer+electronics&qid=1689180534&sprefix=buzzer+elec%2Caps%2C150&sr=8-3"> Link </a> |
| 1K Resistor | Slows Down the Electrical Current | $5.99	 | <a href="https://www.amazon.com/EDGELEC-Resistor-Tolerance-Multiple-Resistance/dp/B07QG1V4YL/ref=sr_1_4?crid=3EFHJNWIP3LWT&keywords=1k%2Bresistor&qid=1689180561&sprefix=1k%2Bresistor%2Caps%2C193&sr=8-4&th=1"> Link </a> |
| Male to Male Wires | Wiring Components | $9.99	 | <a href="https://www.amazon.com/Elegoo-EL-CP-004-Multicolored-Breadboard-arduino/dp/B01EV70C78/ref=sr_1_4?crid=2E8KWUHA2SB4V&keywords=male%2Bto%2Bmale%2Bwires&qid=1689182362&sprefix=male%2Bto%2Bmale%2Bwires%2Caps%2C172&sr=8-4&th=1"> Link </a> |
| Female to Male Wires | Wiring Components | $9.99	 | <a href="https://www.amazon.com/Elegoo-EL-CP-004-Multicolored-Breadboard-arduino/dp/B01EV70C78/ref=sr_1_4?crid=2E8KWUHA2SB4V&keywords=male%2Bto%2Bmale%2Bwires&qid=1689182362&sprefix=male%2Bto%2Bmale%2Bwires%2Caps%2C172&sr=8-4&th=1"> Link </a> |
| Breadboard | Prototyping and Base for Circuit | $12.99	 | <a href="https://www.amazon.com/EL-CP-003-Breadboard-Solderless-Distribution-Connecting/dp/B01EV6LJ7G/ref=sr_1_4crid=2JO3WCBVW2ZO5&keywords=breadboard&qid=1689182601&sprefix=breadboar%2Caps%2C152&sr=8-4&th=1"> Link </a> |
| Clear Acrylic Box | Enclosure | $16.99	 | <a href="https://www.amazon.com/Hewomate-Acrylic-Display-3-9x3-9x3-9-Containers/dp/B09YVLXYC8/ref=sr_1_2crid=1KZVRMN2WVN3I&keywords=acrylic+box+3.9+x+3.9+x3.9+in&qid=1689809468&sprefix=acrylic+box+3.9+x+3.9+x3.9+in%2Caps%2C144&sr=8-2"> Link </a> |
| Stencil Making Sheet | Diffusing Light | $13.99	 | <a href="https://www.amazon.com/Translucent-Stencil-Gyro-Cut-Template-Material/dp/B08PVYHH4M/ref=sr_1_5crid=2WLCSK4EWCFYZ&keywords=banltre+10+sheets+10+mil+mylar+sheet&qid=1689809595&sprefix=banltre+%2Caps%2C132&sr=8-5"> Link </a> |



