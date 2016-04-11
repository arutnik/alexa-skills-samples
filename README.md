# alexa-skills-samples

Amazon Alexa has a lot of verbose documentation, so I set up this page as a high level walkthrough of how to get started with Alexa as a developer.

## Alexa Skills Kit (ASK)
Alexa, the voice personality of Echo and other Amazon voice-enabled devices, has her capabilities broken down into 'skills'. A skill is one subject, knowledge area, or functional tool that Alexa can understand and fulfill. Some built-in skills are like getting the weather and getting sports stats. 

Developers can create and register *custom skills* and *smart home* skills.

*Custom Skills* allow the user to say something like 'Alexa get the high tide for Seatle from TidePooler'. This is the standard interaction model that includes the wake word 'Alexa' the skill name 'TidePooler' and the request ' high tide for Seatle' plus some interchangeable filler words.

_Custom Skills_ have two main requirements:

- An interaction model - this configures what utterances Alexa can understand and how each one should be interpreted into a data model.
- A back end that can receives the request, processes it, and returns a result Alexa can speak to the user. This can be hosted as an AWS lambda function or as any web-accessible service that follows the alexa REST API.
![architecture](https://raw.githubusercontent.com/arutnik/alexa-skills-samples/master/images/askarchitecture.png)

### Getting Started with 'Hello World'

To get Amazon's Hello World sample running you'll need the following requirements:

- Amazon Developer Account
- Java 8 JDK
- Maven command line tool

Clone the repo and follow the steps at https://github.com/amzn/alexa-skills-kit-java/tree/master/samples/src/main/java/helloworld

## Alexa Voice Services (AVS)
Alexa Voice services allows hardware manufacturers / hardware DIYers to add Alexa voice capability to their device that has a microphone and speakers. It is not a means to add voice functionality to mobile apps.
Details: https://developer.amazon.com/appsandservices/solutions/alexa/alexa-voice-service
