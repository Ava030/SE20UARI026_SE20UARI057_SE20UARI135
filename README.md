# Fingerprint Authentication with LED Feedback System using Raspi and Adafruit

This script is designed to interface with a fingerprint sensor, allowing users to enroll, search, and delete stored fingerprint templates. The program provides real-time feedback through an LED — lighting up or blinking based on authentication success or failure. Additionally, security measures have been implemented to handle consecutive failed attempts, triggering a timeout to prevent rapid, repeated unauthorized access attempts.


## Overview  
### Components Involved 
Raspberry Pi, Fingerprint sensor, Jumper wires, Power source, Monitor 

### Hardware Connection
Connect the ground, power, serial communication pins of the fingerprint sensor module to the Raspberry Pi using jumper wires.

### Software and capturing fingerprints 
Connect the Adafruit fingerprint sensor and LED to the Raspberry Pi

1. Open terminal on the Raspberry Pi and install necessary libraries for the fingerprint sensor i.e Adafruit

```pip3 install --user adafruit-nrfutil```

2. Clone this repository

``` git clone https://github.com/Ava030/SE20UARI026_SE20UARI057_SE20UARI135 ```

3. Navigate to the directory

   ``` cd Raspi ```

4. Install the required libraries

   ``` pip3 install -r requirements.txt ```

5.  Run the script

``` python3 fingerprint_sensor_with_led_and_timeout.py```




## Working of  fingerprint recognition for authentication : 
After launching the script:

Use 'e' to enroll a new fingerprint.

Use 'f' to find and authenticate a stored fingerprint.

Use 'd' to delete a stored fingerprint.


LED feedback will provide a clear indication of the status of each operation. It will:

Blink fast for an error.

Blink slowly when waiting for a fingerprint.

Light solid for a few seconds if access is granted.




## Value Proposition
#### Fingerprint Authentication: 
Enables secure user verification through fingerprint enrollment and scanning.

#### Security Features: 
Includes configurable security measures to deter unauthorized access, including a threshold for failed attempts and a timeout mechanism.

#### User-Friendly Interface:
Offers a straightforward console interface for fingerprint management, with LED feedback.





