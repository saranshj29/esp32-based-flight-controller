# esp32-based-flight-controller
# ESP32 flight controller
I have chosen ESP32 as a flight controller mainly because of its cost, wifi & BLE capabilities, and 80MHz clock speed which is 5 times faster than Arduino. 

## Code files
1. Anglemode_flightcontroller_ver3 -  This is the complete code for the ESP32 flight controller, you may have to upload additional libraries in your Arduino ide. Before uploading the code in the ESP32, keep the quadcopter on a spirit-level surface, when the code is uploaded in the ESP32, Make sure to give an initial 10s calibration time for the quadcopter to calibrate Gyro, now after 2 LED blinks on the pin15 the quadcopter is ready for flight.
2. receiver_pwm_esp32 - This code is independently to test the receiver & transmitter signals on serial monitor. connect the receiver to the esp32 board as mentioned in the schematic.
3. measure_angles_mpu - IMU angle checker, connect the imu to the esp32 via the i2c protocal as mentioned in the schematic.
4. Motors calibration - The motor's ESCs have to be calibrated before the flight, such that they start simultaneously, run this code first and calibrate your ESC as per the proper procedure.
# note- some parts of code have been taken from different sources for more depth about code please check them out
