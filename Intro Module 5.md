# Module 5

## Theres an API for that: Objectives
1. Explore the purpose and benefits of APIs
2. Compare Cloud Endpoints and Apigee API Management
3. Examine Pub/Sub, a Google Cloud Tool to handle distributed message-oriented architectures at scale

--------------------------------------------------------------------------------------------------------------------------------

## Purpose of APIs

#### What is an API?
An API or Application Programming Interface, is a tool that allows different software to communicate with other each and exchange data and perform actions
by sending/recieveing requets.

Now, the Rest API is the most common API format tool and is what most APIs are bult upon:

![REST Api](https://i.imgur.com/NbtV9NI.png)

---------------------------------------------------------------------------------------------------------------------------------

## Cloud Endpoints

Is a distributed API management system, it runs using its own proxy on a docker container
it features:
- An API console, hosting, logging, monitoring, and other features
- Use with any APIs that support the OpenAI specification
- Supports applications running in App Engine, Google Kubernetes, and Compute Engine

---------------------------------------------------------------------------------------------------------------------------------

## Pub/Sub

Pub/Sub is short for Publisher/Subscriber - Publish messages to subscribers.

Pub/Sub Features:
- Ensures at-least-once delivery
- No provisioning is required
- APIs are open
- Global by default
- Offers end-to-end encryption

#### Pub/Sub architecture
![pub/sub](https://i.imgur.com/87t2tNX.png)


Then a topic is a central element of a Pub/Sub

[Subscriber] - is at the top here

^ a Topic will point to the subscriber

Topics and subscribers are decoupled





One of the early stages of the data pipeline is data ingestion, where data is received. 

Now what are some challenges to data ingestion:
1. Data can be streamed from many different methods and devices
2. It can be hard to distribute event messages to the right subscribers
3. Data can arrive quickly and at high volumes
4. Ensuring services are reliable, secure, and perform as expected






