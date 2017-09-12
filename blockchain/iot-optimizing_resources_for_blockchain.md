# Prospectus:
## IOT hardware usage optimization for judicious usage 
## Operations performed on IOT devices to get best lifespan and outcome
## Solve the need for security at minute level without being computationally expensive

## Problem:
There isn't a way to trust the data coming from an IOT device.
------------------------------------------------------------------------------
For usage of public key cryptography, data to be sent from the IOT device ought to be encrypted with the private key(digital signature) of the device.
> Recursive functions computationally expensive (in cryptography)

IOT devices cannot be used for encrypting data induvidually because their lifespan gets affected by the intese computation performed by the recursive functions in public key cryptography.

### Example:
If 100 IOT devices are transmitting data, each device encrypting data would do so prior to each transmission every second.

Multiple transmissions would imply multiple signing each drastically reducing the lifespan of the device.

# Goal:
The goal is to obtain a model which will allow the data transmitted to be trusted with minimum liabilty.

-------------------------------------------------------------------------------

# Solutions:
1. Using a master slave mechanism to encrypt data from a number of IOT devices 
2. Using a rotating master mechanism to ensure optimum life cycle usage amongst all devices
3. Using a neural net to detect anomalies and discard them
4. Using a priority level based network


