Problem Definition:<br>
The current project is essentially built to be focused upon selection of a certain  type of crop suitable to a farm based on the conditions prevailing in the farm. 
Many  sensors, methods and technologies have been used to collect the data from the field and  this data is used for picking the appropriate crop. 
Moreover, the inclusion of the cloud  brings a remote monitoring advantage where the requirements and circs can be  reviewed every so often. 
Also, the data that has been accumulated is displayed in  various graphs showing comparison from past times to recently recorded moments such  that the trends in the farm can be judged. 

Hardware Requirements <br>
• Raspberry PI 3 
• DHT11 sensor 
• Humidity sensor 
• Rainfall sensor 
• Soil moisture sensor 
• pH sensor <br>
Software Requirements <br>
• Raspbian OS 
• ThingSpeak Cloud 
• HTML/CSS 
• JavaScript<br>
Languages Used <br>
• Python<br>


Proposed System <br>
• It collects the prevailing conditions of temperature and humidity continuously. 
• It collects the pH data of the soil to determine the acidity, alkalinity of the soil. 
• The moisture levels of the soil at all times is collected to know if that serves the  requirement of a certain crop type. 
• The collected data is sent into a cloud for the purpose of centralizing the data  such that it can be accessed anywhere. 
• The data from temperature, humidity, pH, soil moisture sensors are aggregated  to predict the type of crop that suits a farm. 
<br><br>
Modules<br>
This  project is divided into four significant modules. <br>
• The first module deals with the connection of sensors with Raspberry Pi and  make interactions with its components to work on it. The DHT11, soil moisture,  pH sensors are connected to the Raspberry Pi and this in turn is connected to a  monitor with a HDMI cable, this works as a means to display the actions  performed on the microprocessor. <br>
• In the second module, we embed our cloud credentials and requirements in the  code by creating appropriate cloud channels and fields as required so that the  generated data is accommodated in the respective fields in the cloud and this  can be accessed through the cloud platform provided by thing speak. <br>
• The third module is about building a model that has the capability to predict the  crop type by applying KNN algorithm on the farm data values stored in the  cloud against a predefined dataset. Once the analysis is performed the crop  suitable for the soil is predicted and the model is first trained with the data we  have and then the data we obtain through the farm is used for testing. The more  data we get to collect, the more accurate the model will be.<br> 
• In the fourth module, we send the crop prediction result as a notification to the  farmer through the mail. <br>
• The visible module or the application is where we deploy a webpage and  provide a privilege to the farmer to view his farm parameters at any time.
