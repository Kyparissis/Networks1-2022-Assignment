# Computer Networks I - ASSIGNMENT

## JAVA SERIAL COMMUNICATIONS PROGRAMMING

> Assignment of the **Computer Networks I** Course  
Department of Electrical and Computer Engineering @ Aristotle University of Thessaloniki   
*{Spring Semester 2021-2022}* 

This Network Programming Assignment aims at:
- Developing an experimental network application using Java.
- Learning about the mechanisms of the asynchronous serial communications in practice.
- Collecting statistical measurement values of some parametres that contribute, simultaneously with other, at the configuration of the communication quality on real-life computer communication channels.    


---
>> **Assignment Instructions** can be found [**HERE**](https://github.com/Kyparissis/Networks1-2022-Assignment/blob/main/Assignment-Instructions.pdf) *(Greek)*. 

For this assignment we used the virtual modem [Ithaki-Smart-Modem](https://github.com/Kyparissis/Networks1-2022-Assignment/blob/main/lib/ithakimodem.jar) to communicate with the virtual lab of this course.    
The object class ```Modem.class```  provided by Ithaki's web server allows the serial communication of a PC with a local virtual modem and through that the communication with Ithaki's server using a typical Internet connection (Not a dialup DSL connection).   
 
We create this modem in our Java source code to work with it using the line:   
```Modem modem = new Modem();```   
Then, the source code:      
>> The **SOURCE CODE Project folder** can be found [**HERE**](https://github.com/Kyparissis/Networks1-2022-Assignment/blob/main/Assignment-Instructions.pdf).
- Uses the ```echo_request_code``` code to receive Echo type packets for at least 4 minutes, parses them and then calculates the system's response time.   
Then we create a scatter chart, using Excel, to analyse our system.
- Uses the two ```image_request_code``` codes to receive images taken by the virtual lab's `VideoCoder` (One code gives an ERROR FREE image, the other one gives a WITH-ERROR image).
- Uses the two ```gps_request_code``` codes to receive [NMEA Protocol](http://www.nmea.org/) GPS points' packets from a pre-saved route, parses those point's packets AND then requests an image/screenshot from Google Maps pin-pointing 5 points with distance of at least 4'' between the one to the next one.
- Uses the two ```ack_result_code``` and ```nack_result_code``` codes code to receive ARQ type packets for at least 4 minutes, parses them and then uses an ARQ - Stop and Wait algorithm to check for errors and either re-requests the same packet or requests a new one. Then, also, calculates the system's response time.   
Then we create a scatter chart, using Excel, to analyse our system.   
Fially we create a histogram, using Excel, to find the probability distribution of the number of re-requests per packet, due to errors.
- ...

---
## Output

### Session 1
[**HERE**](https://github.com/Kyparissis/Networks1-2022-Assignment/tree/main/sessions-output/session-1%4012-04-2022).
### Session 2
[**HERE**](https://github.com/Kyparissis/Networks1-2022-Assignment/tree/main/sessions-output/session-2%4015-04-2022).

---

## Reports
...

---

## How to use
...

---
---
## TO DO:
- ADD INSTRUCTION ON HOW TO USE THE SOURCE CODE OF THIS PROJECT
- MAKE A BETTER README.md
