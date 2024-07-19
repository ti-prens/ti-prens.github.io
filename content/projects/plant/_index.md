---
title: "Digital gardener"
date: 2017-08-02
tags: ["project","sample","college"]
genre: "project_school"
draft: false
type : "page"
---


**Digital Gardener**
--------------------

To the question:  
> "How many sensors could you use to take care of a plant?"  

I answered **YES!**


Welcome to my adventure in tech-powered gardening! Instead of relying on a green thumb, I’m using a handful of sensors and a dash of programming magic to keep my plant happy. Here’s a peek at how I turned a regular plant into a tech-savvy green friend. No plant were harmed during this process... I think.

### The Project

Our mission? To create a system that ensures a plant is well taken care of with minimal human intervention. While connected gardens aren't groundbreaking, this project served as a playground for experimenting with sensors, actuators and even the web.

![plant](/img/not_feature_plant_2.jpg)

### What We Did

We kept things straightforward to meet our deadlines:
1. **Read sensor data** – Check!
2. **Send data to our local server** – Check!
3. **Show important info on a dashboard** – Check!
4. **Display useful info on a screen** – Check!
5. **Water the plant** – Check!

![flow](/img/Rapport_BE_Realisation_systemes/flow_of_data.png)

### Tools and Tech

Here’s a look at the hardware we used:

- **STM32 Microcontroller** – The brain of our operation.
- **LCD Display** – Displays sensor readings.
- **Various Sensors** – Measures soil moisture, air humidity, temperature, and even water levels in the tank[^tank].
- **WiFi Shield** – I did not find a better excuse to learn some JavaScript and Angular.
- **Peristaltic Pump** – Waters the plant as needed.

### How We Did It

**0. Managing and Version Control**  
As a team of two, [Mouloud Ziane](https://www.linkedin.com/in/mouloud-ziane-52129a14b/) and [I](https://www.linkedin.com/in/prince-jacquet/) used Trello and (git) GitHub to collaborate.  
![trello](/img/Rapport_BE_Realisation_systemes/trello.png)

**1. Setting Up the STM32:**  
Using [CubeMX](https://www.st.com/en/development-tools/stm32cubemx.html), I configured the [STM32 (a nucleo dev board)](https://www.st.com/en/evaluation-tools/nucleo-l152re.html#documentation) to handle our sensors, screen, and pump. We then divided the development of the drivers between ourselves.

**2. On the Sensors:**

- **RGB Color Sensor** – Checks if the plant is receiving the right light. (Disclaimer: "right" light is somewhat subjective... I’m no botanist 😅)
- **Water Level Sensor** – Determines if the water tank needs to be refilled.
- **Soil Moisture Sensor** – Monitors soil hydration.
- **Air Moisture/Temperature Sensor** – It does exactly that ^^.

**3. The Pump:**  
We connected a mini peristaltic pump to automatically water the plant. This required some basic wiring and using a relay to control it.

**4. WiFi Connection:**  
The WiFi Shield V2 enabled us to send data to the cloud[^cloud] and receive commands. We configured it to connect to our local network and transmit data to our dashboard.

**5. Web Development:**  
I created a full-stack web application to visualize the plant’s status and manage its care. This involved:
- **Frontend:** Built using Angular to display real-time data from the sensors.
- **Backend:** Developed with Node.js to handle data requests and control the WiFi Shield.
- **Database:** Utilized a lightweight database to store historical data for analysis. Also called a file. Yes Sir !.

![web dev](/img/Rapport_BE_Realisation_systemes/web_dev.png)

### Code and Control

We wrote straightforward code to manage everything:

- **Initial Setup:** Configured pins and set up peripherals.
- **Sensor Reading:** Collected data from sensors and converted analog signals to digital values.
- **Displaying Data:** Used the LCD to show sensor readings and system status.
- **WiFi Communication:** Used the WiFi module to send and receive data.
- **Dashboard Setup:** Created a web application to display sensor data and system status.
- **Watering:** Controlled the pump with a relay based on soil moisture readings.


### The Takeaway

This project was a fun blend of electronics and plant care.
It was exciting to see, or at least imagine, how my newly acquired tech skills could interact with the real world, from managing sensors to being a full fledge gardener.
Plus, diving into my first Angular/Node.js stack was a great learning experience. I enjoyed the challenge, but I must admit, I still prefer C! 🤣

So, there you have it! A tech-filled journey where a few sensors and a bit of code ensured a plant’s needs were met in style.


Feel free to dive into our [GitHub repo](https://github.com/PrinceJacquet/STM32_27.git) for more details, or watch our [project video](https://youtu.be/Y9t1PGNbQd0) for a closer look at the setup.

Happy gardening... tech-style ^^ ! 🌱💻

[^cloud]: Psstt ... The cloud is just my own computer over the network 😆.
[^tank]: The tank is just a glass of water, man.

<iframe src="https://giphy.com/embed/3ZF400H2Jh5Sg" width="480" height="360" style="" frameBorder="0" class="giphy-embed" allowFullScreen></iframe>