# System Architecture of Ride Sharing App
## Introduction
Its an architecture document for a Ride Sharing App.

### Document Overview
This document describes the architecture of Ride Sharing App.
It describes:
- A general description of system and requirements
- The logical architecture of software, the layers and top-level components
- The physical architecture of the hardware on which runs the software
- The justification of technical choices made
- The traceability between the architecture and the system requirements.

## Functional and Non Functional Requirements
### Functional Requirements
1. User Registration
    - User must be able to register for the application through a valid email or phone. User should be get the activation link or activation code on mail or phone after registration for validation.

2. Choose Route
    - User must be able to select the pickup and drop location. 

3. Notification
    - Ride App registered driver nearby the pickup locations should be notified for pickup request. 
    - User should be notified if any of the driver accept the pickup request with the current location of the driver.

4. Confirm the ride
    - User must be able to select the ride from the list of accepted request and confirm for the ride.
    - Ride App registered driver need to be notified after the confirmation.
    - Total cost for the ride need to be calculated and user should have the option to pay with wallets/banks. Cash can be the option and need to pay after he gets picked up for the ride.

5. Feedback and rating
    - User must be able to provide feedback regarding the ride and the person.

### Non Functional Requirements
1. Privacy 
    - Password for the app must be highly secured Min 8 Characters and Capital/Special Character and Digit validation. 
    - Digital Wallets and Bank information should be highly secured and should avoid the saving of those information on the application. 
    - Try get these information on the fly using the APIs and remove the information after its use. 

2. Robustness 
    - DataServer must have specific backup schedule so as to recover the history on any kind of system crash.
    - Application is more over the cash or money transaction so need to log every information regarding the transaction as well as the location of the rider and driver as much as possible

3. Performance 
    - Application must be as quick as possible. 
    - Notification should be instant so as to robust the app use.
