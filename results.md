[Home](./index.md)/[Introduction](./introduction.md)/[Deliverables](./deliverables.md)/[Results](./results.md)/[About Us](./aboutus.md)/[Contact](contact.md)

### Results and Discussion

From the testing results, it can be concluded that a fall generates acceleration values that are much higher than normal motions such as walking and sitting; therefore, we can design an algorithm based around a peak threshold value of 600ms2. Normal motions resulted in values between 300-400ms2 while falls generate as much as 1000ms2 or even higher. The peak threshold was chosen to assure that we catch every fall, minimizing ‘false’ positives. 

In addition, the fall detection algorithm does not have the capability catch slower falls due to the threshold acceleration value. Since it is limited to only acceleration value, in the future it is important to utilize on-board gyroscope to detect the user’s orientation so that the device can have another basis to detect a fall based on user’s position. 

From the study, another observation that was made was the placement of the device on the user. It was found that when the user fell on the side that the device was positioned (i.e.  right side of the waist), the acceleration was much more skewed. The reasoning for this is because the device was not placed at the user’s center of gravity. 


### Conclusion

The self-activating fall alarm has been successfully developed using a 9DOF Razor IMU which incorporates three sensors, a triple-axis - Gyroscope, Accelerometer and Magnetometer - to yield nine degrees of inertial measurement. The outputs of all sensors are processed by an on-board ATmega328 and output over a serial interface to a PC using a Bluetooth module. Then a C++ program on the PC stores the serial data within a text file and analyzes the data using a fall detection algorithm. When the fall detection algorithm recognizes a peak acceleration value that exceeds the predefined fall threshold, the program will send an email and SMS to the caregiver to help the user

The self-activating fall alarm meets several of the objectives stated earlier in the report. This device has completely taken the user out of the picture and is self-activating. Additionally, the device can send multiple alerts to a handful of caregivers to notify when user has fallen within 10 seconds (depending on Wifi strength). If the user is inactive for a long period, the system also recognizes this as problematic and will also alert caregivers. The algorithm save the pre-fall data for physicians to analyze which actives are associated with the most serious falls and which falls result into the most traumatic injuries.  

The next phase of this project should be aimed in erasing ‘false-positive’ falls. To accomplish this, the fall algorithm should integrate the gyroscope data as the second basis for detecting false. This will greatly reduce ‘false-positive’ falls, requiring the device to consider the orientation of the user before declaring a fall. Incorporating a GPS module would be beneficial for this device. When an SMS is sent to caregivers, the geographic data of the user can also be attached in the test. Other improvements include switching to Wife to increase range of connectivity and replacing PC with a Raspberry Pi; having the device connect to a PC is not practical to market this product and will improve efficiency of the product. Lastly, the outer appearance of the overall device should be targeted. Design a customize box which is compact, lightweight system is very crucial to the overall success of the device. 


  
