# Resolving Architecture Documentation
Documentation on how to use these services.

## Quick Start
Currently the best method to try out the services is to pull down the projects of interest.
Look at each project's Maven pom and ensure you have all of the required projects.
Compile each project based on its order of dependency. Create a daemon and start the service bus
registering services after successful startup. Service Bus will soon have a Daemon so that it 
will be installed as an OS service and a Server Socket for administering the bus and calling it
using a Client Socket connection for local connections.


## Foundation
Most projects in Resolving Architecture's GitHub space were designed for deployment to the Service Bus project.
The Service Bus projects uses the SEDA Bus project as its Message-Oriented Middleware (MOM).

The original services are Java based. Java implemented projects are slowly being implemented in Rust for the OS project
(version 0.8) and in Typescript for use in browsers.

* SEDA Bus is the foundational library for dapps where all message integration occurs between services.
    * [Java](https://github.com/resolvingarchitecture/seda-bus-java) - Fully working
    * [Rust](https://github.com/resolvingarchitecture/seda-bus) - Started but not yet fully tested
    * [Typescript](https://github.com/resolvingarchitecture/seda-bus-ts) - Project created but not implemented
* Service Bus sits on top of SEDA Bus using it to pass messages between services. The service bus provides registration of services and a simple router to route messages between services. More complex routing can be provided as a service. Service monitoring and adminstration is handled by the service bus.
    * [Java](https://github.com/resolvingarchitecture/service-bus-java) - Fully working
    * [Rust](https://github.com/resolvingarchitecture/service-bus) - Started but not yet fully tested
    * Typescript - Not yet started

## System Services
No system level services to date. This is expected to change as needed by pulling functionality out of the
utility libraries making them into services.

## Privacy Services
* TOR
* I2P

## Censorship-Resistance Services
* Network Management
* Bluetooth
* WiFi
* Satellite
* Full-Spectrum Radio
* ECCM
* LiFi - Light Fidelity

## Financial Services
* Bitcoin
* Bisq
* Lightning

## Social Media Services
* Messenger

## Decentralized IoT (DoT) Services
* Content Distribution

## Services in Heavy R&D


## Future Services

