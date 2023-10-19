# Super App Architecture Overview

The Super App employs a modular architecture that offers both flexibility and scalability. This design has multiple modules as described below. The utilization of micro-frontends and microservices allows different teams to work on separate components independently.

![Architecture](/architecture.png")


## Main Components

### **Super App**
The Super App is the central hub that houses all other modules and core components. It acts as the overarching application where everything else resides. The bundle being submitted to the app store will be built using this module.


### **Native Modules + RN Core**
These are the foundational elements developed using React Native (RN Core). They serve as the backbone for the core functionalities of the Super App.


### **Foundational Features**
These are the non-modular, essential features that are integral to the Super App itself, suich as navigation, dashboard rendering, etc.


## Micro-Frontends

### **Auth Micro-frontend**
This is a self-contained unit responsible solely for authentication processes, including login, registration, and user verification. Since being a critical module, this will be combined as part of the super app bundle.


### **Settings Micro-frontend**
This is also a self-contained module is crafted for managing user preferences, app configurations, and other customization features. Again, bundled along with the super-app


### **Credit Card Micro-frontend**
This module handles all aspects related to credit card application and status tracking. This module is deleveloped, built and distributed independently and remotely loaded into the app.


## Integrated Views and PWAs

### **Binance Web View**
This integrated web view showcases either the entire Binance website or PWA can be embedded within the Super App.


### **Crypto PWA**
This Progressive Web App focuses on cryptocurrency-related services and information, which is hosted externally on Firebase. This module also demonstrates the ability to exchange data between super app and the micro-frontends.


### **App Bundle Storage and Distribution**
The remote bundles distribution are managed by utilizing the following 2 services: 

- **Amazon CloudFront**: A Content Delivery Network that ensures global content delivery with minimal latency.
  
- **Amazon S3**: Used for storing app modules and other static assets.


### **Personalization Microservice**
This backend service is tailored to collect user data and preferences for providing a personalized user experience within the Super App.

### **Catalog Microservice**
This standalone service manages a catalog of items, products, or services, and can cater to various modules within the Super App.

## Repository Structure


