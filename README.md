# Eurotech-Live-Objects-connector-for-IoT-edge-computing

## Table of contents
* [General info](#general-info)
* [Technologies](#technologies)
* [Requirements](#requirements)
* [Configuration](#configuration)

## General info
![Architecture](/assets/architecture.png)
In this repository you can find how to connect Live Objects to the Everyware Cloud using node-red connector. The goal of the project is to synchornize the data between two former mentioned platforms.


3 Main functionalities:
* **devices list synchronization** - every device created in EC will automatically apear in LO as well as every deleted device in EC will disapear from LO.
* **Data transfer from Live Objects to Everyware Cloud** - Sending data to EC devices using the LO commands system.
* **Data Transfer from Everyware Cloud to Live Objects** - Forwarding the End-Devices data form EC to LO.

## Technologies
* Node Red

## Requirements
* Live Objects Account
* Everware Cloud Account
* Everyware Software Framework Gateway
* End-Device

## Configuration
The Node Red can be configure by importing the **EC<>LO-command-handler.json** and  **EC<>LO-connector.json** to two separate flows. In each one it is crucial to change the LO API KEY and EC API credencials in the follwoing function nodes: **Pass Credentials, Pass API Key, Set LO API Headers and URL** and in the follwoing MQTT nodes: **connector/v1/requests/command, MQTT**

  
