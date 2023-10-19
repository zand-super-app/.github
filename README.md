# Super App Concept to Implementation

Super App employs a modular architecture that offers both flexibility and scalability. Utilizing micro-frontends and microservices allows different teams to work on separate components independently.

![Architecture](architecture.jpg 'Architecture')

## Table of Contents
- [Super App Concept to Implementation](#super-app-concept-to-implementation)
  - [Table of Contents](#table-of-contents)
  - [Main Components](#main-components)
    - [Super App](#super-app)
    - [Native Modules + RN Core](#native-modules--rn-core)
    - [Foundational Features](#foundational-features)
  - [Micro-Frontends](#micro-frontends)
    - [Auth Micro-frontend](#auth-micro-frontend)
    - [Settings Micro-frontend](#settings-micro-frontend)
    - [Credit Card Micro-frontend](#credit-card-micro-frontend)
  - [Integrated Views and PWAs](#integrated-views-and-pwas)
    - [Binance Web View](#binance-web-view)
    - [Crypto PWA](#crypto-pwa)
  - [App Bundle Storage and Distribution](#app-bundle-storage-and-distribution)
  - [Backend Microservices](#backend-microservices)
    - [Personalization Microservice](#personalization-microservice)
    - [Catalog Microservice](#catalog-microservice)

## Main Components

### Super App

The Super App is the central hub that houses all other modules and core components. It acts as the overarching application where everything else resides. The bundle submitted to the app store is built using this module.

### Native Modules + RN Core

Developed using React Native (RN Core), these foundational elements serve as the backbone for the core functionalities of the Super App.

### Foundational Features

These are the non-modular, essential features integral to the Super App, such as navigation and dashboard rendering.

**Repo URL:** [Super App Repository](https://github.com/zand-super-app/super-app)

## Micro-Frontends

### Auth Micro-frontend

Responsible solely for authentication processes including login, registration, and user verification. Bundled as part of the super app.

### Settings Micro-frontend

Crafted for managing user preferences, app configurations, and other customization features. Bundled along with the super app.

### Credit Card Micro-frontend

Handles all aspects related to credit card application and status tracking. Developed, built, and distributed independently.

**Repo URL:** [Credit Card Micro-Frontend Repository](https://github.com/zand-super-app/credit-card-micro-frontend)

## Integrated Views and PWAs

### Binance Web View

This integrated web view can showcase either the entire Binance website or a PWA embedded within the Super App.

### Crypto PWA

Hosted externally on Firebase, this Progressive Web App focuses on cryptocurrency-related services and information.

**Repo URL:** [Crypto PWA Repository](https://github.com/zand-super-app/crypto-pwa)

## App Bundle Storage and Distribution

Remote bundles are distributed through:

- **Amazon CloudFront:** A CDN that ensures global content delivery with minimal latency.
- **Amazon S3:** Used for storing app modules and other static assets.

## Backend Microservices

### Personalization Microservice

Tailored to collect user data and preferences for a personalized user experience within the Super App.

**Repo URL:** [Personalization Service Repository](https://github.com/zand-super-app/personalisation-service)

### Catalog Microservice

Manages a catalog of items, products, or services, catering to various modules within the Super App.

**Repo URL:** [Catalog Service Repository](https://github.com/zand-super-app/catalog-service)
