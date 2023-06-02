# Industrial Edge - Bring your own application

## Steps

1. Installation
   - Build Application
   - Use Hello World
   - Build Docker
     - Upload app to the management
   - Connect Publisher
   - Upload
     - Install App on edge Device
     - Use App

## Requirements

- Download https://github.com/industrial-edge/hello-world to your development folder
- Install Docker engine and allow communication from outside
- Industrial edge management - Up and running
- Industrial edge Device - Up and running

## Build Application

1. Open Visual Studio Code
2. Open folder in Visual Studio Code:
   - Development folder
3. Build Docker in Visual Studio Code
   - Right click on "hello-world"
   - Open in Integrated Terminal
     - Build Docker image by typing:
       ```
       Docker-compose build
       ```
     ![Build Docker](assets/20230601_162004_image.png)

## Create New App in the Industrial Edge Management

1. Login to the management
2. Go to App-Projects > Create project
3. Create a new app in the folder. Name it "hello-world"
4. Fill in all the fields
5. Create

![Create App](assets/20230601_162147_image.png)

## Setup the Publisher

1. Open the publisher
2. Connect Docker engine
   
   ![Connect Docker Engine](assets/20230601_164109_image.png)
   ![Connect Docker Engine](assets/20230601_164123_image.png)
3. Connect publisher to the management
   
   ![Connect Publisher to Management](assets/20230601_164151_image.png)
4. In the publisher, open Project > Hello-World
5. Add new app version
6. Import the docker-compose file at the import YAML button
   - Select the docker-compose.yml in the hello-world folder
   - The warnings can be ignored
7. Configure the reverse proxy of the hello-world service. Click the edit button to change settings
  
  ![Configure Reverse Proxy](assets/20230601_164340_image.png)
8. Go to "network" and set up the following
   
   ![Set up Network](assets/20230601_164356_image.png)
9. Click on "+" and you should see
  
  ![Add Network](assets/20230601_164420_image.png)
10. Press "Save"
11. Click "Review" and "Validate and Create"
12. Start upload to transfer to the management

## Install Application on Device

1. Go to the IE Management
2. Go to App Projects > Project
   - Open app > Hello-World
   - Publish the latest version to be used for everybody!
     
     ![Publish Latest Version](assets/20230601_164703_image.png)
   - Press on the download icon and select your edge device
     
     ![Download Icon](assets/20230601_164732_image.png)
   - Install on your edge device

## Edge Device

Go to your edge device and the new app should be available

- [x] Dockerized an app
- [x] Uploading an app
- [x] Publishing App for other users
- [x] Set up a reverse Proxy
