# Disertatie-Lucrare-Finala

My dissertation project is an IoT application, an intelligent assistant (powered by ChatGPT) with both hardware and software components, designed to help a user take care of a plant to a greater or lesser extent.  
The system integrates several modern technologies – sensors connected to a Raspberry Pi board from which data is retrieved using a Python script. This data is stored in a Firebase instance and a user application developed with Java in Android Studio, which is integrated with ChatGPT.  
Here it is a short summary.

![image](https://github.com/user-attachments/assets/a11d952e-693a-4474-b313-3c7b565cc92d)


## Hardware Part

The Raspberry Pi circuit has the following modules conected to it: AM2320( sensor for temperature and humidity), BMP280 ( sensor for temperature and atmospheric preassure), BH1750FVI ( sensor for light intensity), resistive soil moisture sensor, resistive rain sensor, water pump, 3VDC Relay, aditional power source, LED, comparator module LM393, BreadBoard, cables.

![image](https://github.com/user-attachments/assets/497aff9b-68d2-4987-8cf1-944514d652a1)


## Software Part

### Python Script

Flow of the Python Script

![image](https://github.com/user-attachments/assets/206e6610-f36b-4bfb-92ec-35a1d427366c)



### Database Structure

The application uses a Firebase real-time database, which is a NoSQL database type. It has two tables stored in JSON format. Another feature is authentication based on unique tokens implemented through Firebase.  
The DataPrefferenceApplication table contains the care routine generated by ChatGPT, which is regenerated every time a new plant is added to the application.  
The DataPythonRaspberryPi table contains information updated every 5 seconds by the Python script, it primarily includes the data from the board.

![image](https://github.com/user-attachments/assets/49701bf6-98b0-4655-8fbf-66d409c2ae90)

![image](https://github.com/user-attachments/assets/3e71703e-ca68-476e-9c4f-02b4d432bb8e)

![image](https://github.com/user-attachments/assets/e9462b49-f2b7-4214-a526-b20e7333d116)






### Android Application

* Ability to log in/register/reset password
* Viewing real-time data about the plant
* Continuous monitoring of the plant's condition and sending notifications in case of issues
* Uploading a customized care regimen for the selected plant for day/night
* Automatic mode for watering/additional lighting
* Manual mode for setting watering intervals
* Manual control for turning the plant’s additional lighting on/off
* Page for additional care regimen (soil change, propagation, other information)
* Special page dedicated to describing current incidents
* Page with plant recommendations generated by ChatGPT based on the currently selected plant
* Option for live chat with an AI chatbot 24/7 for any botanical questions
* User-friendly and intuitive GUI


#### Login Page

<a href="url"><img src="https://github.com/user-attachments/assets/868ec6bb-046c-4e2a-b58c-b9e2c5146f50" align="left" height="48" width="48" ></a>


#### Register Page
![Screenshot_2024-09-13-10-00-41-56_2c09c55d223b81c223fa6cb6a059c5be](https://github.com/user-attachments/assets/743da9b8-99a3-4cc1-9545-79fb5fe5999a)

#### Forgot Password Page
![Screenshot_2024-09-13-10-00-54-05_2c09c55d223b81c223fa6cb6a059c5be](https://github.com/user-attachments/assets/63611edc-7e30-421c-9338-d48f38ef5b9f)

#### Home Page

#### Issues Page

#### Select Option Page

#### General Informations Page

#### Live Chat Page

#### Recommendations Page










