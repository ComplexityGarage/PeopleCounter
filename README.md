# People Counter  

# Authors  
- Kamil Adach  

# Description of the project  
The project is a system based on the Arduino platform that counts people entering and exiting a room. It uses two HC-SR04 ultrasonic sensors, placed at the entrance, to detect movement and determine the direction in which a person is moving. After identifying the activation sequence of the sensors (e.g., the first sensor detects movement followed by the second), the system appropriately increases or decreases the people counter. The current count is displayed on an LCD screen, allowing real-time monitoring of the number of people in the room.  

# Science and tech used  
The project utilizes the following technologies and solutions:  

- **Arduino Platform**:  
  - A microcontroller (e.g., Arduino Uno or Nano) responsible for processing sensor signals and controlling the LCD display.  

- **HC-SR04 Sensors**:  
  - Two ultrasonic sensors that measure distance by emitting a sound pulse and recording the echo time.  
  - They allow detecting objects (including people) moving within the detection field.  

- **LCD Display**:  
  - A 16x2 screen is used to display the current count.  

- **Code**:  
  - The program is written using Arduino IDE and implements data processing logic, noise filtering (e.g., using median algorithms), and prevents double-counting of the same person.  

# State of the art  
Currently, occupancy monitoring systems are a key component of smart buildings. Among modern solutions, the following stand out:  

- **Computer vision-based systems**:  
  - They use cameras and advanced image processing algorithms, ensuring high precision but involving higher costs and privacy concerns.  

- **Infrared and PIR sensors**:  
  - Often used in building automation but may have limitations in detecting multiple people simultaneously.  

- **Our HC-SR04-based solution**:  
  - **Economical and simple**: Uses inexpensive and easily accessible components.  
  - **Low computational requirements**: Ideal for use in small and medium-sized rooms.  
  - **Scalability**: Can be part of a larger IoT system, integrating data from multiple sensors.  

# What next?  
Future developments of the project may include:  

- **Expanding sensor capabilities**:  
  - Integrating additional sensors, such as PIR or infrared sensors, to improve accuracy and reliability.  

- **Wireless connectivity**:  
  - Adding an ESP8266/ESP32 module to enable remote monitoring and data transmission to the cloud, useful in smart building systems.  

- **Algorithm optimization**:  
  - Improving detection logic, especially when multiple people pass through simultaneously or when interference occurs.  
  - Implementing more advanced filters, such as a median filter, to eliminate incorrect readings.  

- **Enhancing the user interface**:  
  - Expanding the display or creating a mobile application to visualize data and manage the system.  

- **Data collection and analysis**:  
  - Logging room occupancy data for trend analysis and space optimization.  

# Sources  
- **Arduino Official Documentation**: Information on programming and configuring Arduino boards, as well as best practices in microcontroller programming.  
- **HC-SR04 Datasheet**: Detailed technical specifications and guidelines for proper usage of the ultrasonic sensor.  
- **LCD Display Tutorials**: Online guides on connecting and programming 16x2 displays (with or without an I2C module).  
- **Arduino Community Projects**: Contributions and experiences from other creators who have experimented with people-counting systems and movement detection logic.  
