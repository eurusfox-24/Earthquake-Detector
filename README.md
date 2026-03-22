# Arduino Earthquake Detector

This project is an Arduino-based earthquake detector that uses an analog accelerometer to sense sudden motion, triggering a red LED and a speaker alarm. 

**The Story Behind the Project**
We originally set out to build sign language translation gloves. However, practical testing quickly showed us that the flex sensors we had were too unreliable to track fine finger movements accurately. 

Instead of forcing a flawed design, we stepped back and looked at the core technology we knew worked flawlessly: the accelerometer. By pivoting our focus, we successfully repurposed our working hardware into a functional earthquake detector.

*Note: I lost the original GitHub repository for this project, so I have created this new one to replace it. The code provided here is the exact original version we wrote.*

## Components Used
* Arduino Nano
* Breadboard
* Jumper wires
* Accelerometer (analog)
* Small speaker
* Red LED

## How to Replicate

If you want to understand how this system works, the best way is to try it yourself. Follow these steps to set it up.

### 1. Download the Code
Download or clone the main Arduino code file from this repository to your computer.

### 2. Wire the Components
Connect the components to your Arduino Nano using the breadboard:
* **Accelerometer:** Connect the data pins to A0, A1, and A2 (for the X, Y, and Z axes), plus power (5V) and ground (GND).
* **Red LED:** Connect the positive leg to digital pin 8 and the negative leg to ground.
* **Speaker:** Connect the positive wire to digital pin 9 and the negative wire to ground.

### 3. Upload the Code
Open the code in the Arduino IDE software, connect your Arduino Nano to your computer via USB, and click the upload button.

### 4. Test the System
Once the code is running, gently shake or tap the breadboard. If the motion passes the baseline threshold, the red LED will flash and the speaker will play the siren sound.
