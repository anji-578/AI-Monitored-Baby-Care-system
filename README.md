
# AI monitored baby care system

#### OBJECTIVES AND GOAL

 - The objective of our project is to build a smart baby-care/monitoring system, which would monitor the various physical parameters around the baby and inform the parents about it through wireless communication.
 - We intergrated IOT and computer Vision to make an automated system. 
 - In **IOT system** takes cares of physical paremeters of the baby. We have an **Dashboard** in **Arduino IOT** cloud where the sensor data will be uploaded lively and displayed in terms of graphs.
 - In **Computer Vision system** monitor module we will monitor baby movements and using the baby cues we predict the following :- **Sleeping Posture,Hungerness,Tiredness** of the baby.


## Output Screenshots with explanation


## Hardware Implimentation Screenshots

### Block Diagram

![](https://user-images.githubusercontent.com/68511369/221432157-db1bfa4f-21cd-49a0-9485-5a50d1cb476b.png)


#### Hardware Implimentation Snapshot

![Hardware](https://user-images.githubusercontent.com/68511369/221432743-b731d329-9c80-42e2-85a3-e83f88250e85.png)

![NodeMCU](https://user-images.githubusercontent.com/68511369/221432779-8d02b146-1230-4c04-86c4-cf3fe16eb510.png)



#### Arduino IOT Dashboard

![cloud1](https://user-images.githubusercontent.com/68511369/221432798-3265bda5-7b44-48cc-b6b3-b6be733f8f07.png)

![cloud2](https://user-images.githubusercontent.com/68511369/221432820-eeb019f6-c451-4887-b27e-fa61cfe4a936.png)


#### Arduino Code IDE

![arduino code1](https://user-images.githubusercontent.com/68511369/221432887-da0b8802-14e1-4481-9dc6-fb0886f1fa9a.png)

#### IOT Dash Board

##### Sensor values will sent to parents in live in form of messaging
![dash1](https://user-images.githubusercontent.com/68511369/221432917-9e55ebf1-b265-4d8c-bed5-ebe355543bf3.png)

##### Temperature Values viz

![dash2](https://user-images.githubusercontent.com/68511369/221432938-b2e0c1ad-536f-4262-9038-27edccf71b28.png)

##### Humidity Values viz

![dash3](https://user-images.githubusercontent.com/68511369/221432947-92d5c4ff-54e9-42d0-8e69-d7a109a6546f.png)

##### Sound Sensor viz

![dash4](https://user-images.githubusercontent.com/68511369/221432948-4e142a33-bf38-4573-804b-24bfcfed3ca8.png)

##### Switch control where parents can control fan from remote place

![dash5](https://user-images.githubusercontent.com/68511369/221433201-082db43a-fde9-43f5-b3e4-9ad3fd80f22f.png)







### Computer Vision Implimentation Screenshots


#### Computer Vision module flow diagram

![Computervison flow](https://user-images.githubusercontent.com/68511369/221434659-1221200c-1400-4f7f-8fd0-183d528195ad.png)


##### We used **Face,Hand,Pose estimation in Mediapipe Library** to get the ***co-ordinates*** of parts.

 ### Baby Sleep Detection
We will detect if the baby is sleeping or not by taking ***cordinates of the Top point of eye and bottom point of eye*** and find the distance between them ***if the eye is close then distance=0***.

#### FaceMesh for sleep Detection
![FaceMesh for sleep](https://user-images.githubusercontent.com/68511369/221434373-6f4066d2-a87a-4800-85dc-abb6e9790e47.png)

#### Sleep Detection

Sleep is detected if the baby is closing eyes for more then 10secs

![sleep](https://user-images.githubusercontent.com/68511369/221434383-3548da93-b81c-4e54-aaf0-6a6b72d31333.png)

### If the baby is sleeping

##### According to medical studies it is proven that it sleeping by facing head to bed will lead to SIDS and may even cause death sometimes. So we will detect sleeping posture of baby.

#### Face Mesh For Sleeping posture
![Sleep posture mesh](https://user-images.githubusercontent.com/68511369/221434394-6eeb0e8a-8528-4294-9adb-f7bb1242fd21.png)

#### Sleeping Posture Detection
 We will find the ***co-ordinates of left part of mouth to right part of mouth*** if the baby is sleeping backside of camera the visibility range will decrease and ***distance between two points will becomes very less***. So if the become very less we will detect that baby is sleeping wrong position and send the message to parent.

![Sleep posture_detected](https://user-images.githubusercontent.com/68511369/221434397-7e3fcc71-8bf5-455d-a06e-f00fb0124d4e.png)

### If the baby is not sleeping


#### If the baby is not sleeping we will predict 2 factors Hunger and tiredness

### Hunger Detection

  #### Hunger cues of baby.
   - sucking hands
   - Opening and closing of mouth
   - Fist 
If the co-ordinates of hand is close to the mouth for more than 10 sec hungerness is detected.

![Hunger_detected](https://user-images.githubusercontent.com/68511369/221434646-ceb9991b-a9dd-448e-b497-e1a60da0e5bc.png)

### Tiredness Detection


  #### Tiredness cues of baby
   - Pulling eyes and ear
   - Yawning
If the cordinates of the hands coming close to eyes for more than 5secs then tiredness is detected as a result music will switch ON to make baby engaged.

![Tiredness](https://user-images.githubusercontent.com/68511369/221434652-7f3bd81f-65c1-44bd-9229-f967c868c03e.png)
















## Demo



### Demo Video Of Hardware Implimentation
 
[Hardware Implimentation](https://drive.google.com/file/d/1DqrU84B4dkzGGaFUolO8SpNX3P2hNLUA/view?usp=drivesdk)


## TechStack


**MicroController:-** NodeMCU                            

**Sensors:-** Temperature Sensor,Humidity Sensor,Sound Sensor
**Actuators:-** Servo Motors

**Cloud:-** Arduino IOT Cloud

**Open-CV**

**Media Pipe**
## Documentation

[IOT Module Implimentation Report](https://docs.google.com/document/d/1T1OXSsz0NWd27aFLZNAsSF9-amFcS6IL/edit?usp=share_link&ouid=112169638179078369544&rtpof=true&sd=true)

[Computer Vision Implimentation PPT](https://docs.google.com/presentation/d/1WnahRm5PpqrNtc7e6x-cLCaGUmS_jb0g/edit?usp=share_link&ouid=112169638179078369544&rtpof=true&sd=true)
# Hi, I'm Anjani Babu! 👋


## 🚀 About Me
I am a passionate Data enthusiast who loves to work with data.


## 🔗 Links

[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/anjani-babu-janyavula-12b2601b1/)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/AnjaniDS1081)


## 🛠 Skills
Python,MySQL,Data Analyisis,Machine Learning,Computer Vision

