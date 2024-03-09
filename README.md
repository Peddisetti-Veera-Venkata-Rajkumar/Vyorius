This system uses an Arduino board equipped with temperature, humidity, and light level sensors to collect environmental data and transmit it wirelessly to a Python script via Bluetooth Low Energy (BLE). The Python script receives the data, performs basic processing such as averaging multiple readings, and displays the results on the console.

Requirements
Arduino board (e.g., Arduino Uno)
BLE module (e.g., HM-10)
Sensors: Temperature, Humidity, Light Level
Jumper wires and breadboard
Python 3.x
Python libraries: bleak, asyncio, statistics
Arduino IDE
Hardware Setup
Connect the sensors to the appropriate pins on the Arduino board.
Attach the BLE module to the Arduino using the serial pins.
Ensure all connections are secure.
Software Setup
Arduino
Install the Arduino IDE from the official website.
Open the Arduino IDE and install the ArduinoBLE library via the Library Manager.
Load the provided Arduino sketch into the IDE.
Select the correct board and port from the Tools menu.
Upload the sketch to the Arduino board.
Python
Ensure Python 3.x is installed on your system.
Install the required Python libraries using pip:
pip install bleak asyncio statistics

Save the provided Python script to your local machine.
Running the System
Power the Arduino board.
Run the Python script in a terminal or command prompt:
python ble_sensor_script.py

Observe the output in the console. The script will display the processed sensor data.
Troubleshooting
If the Arduino cannot find the sensors, check the wiring and sensor addresses.
If the Python script cannot connect to the BLE device, ensure the BLE module is powered and advertising.
For any serial communication issues, verify the correct port and baud rate are selected in the Arduino IDE.
