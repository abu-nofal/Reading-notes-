# Event Driven Architecture

### Review, Research, and Discussion

1. What’s the difference between a FIFO and a standard queue?
- ![](https://miro.medium.com/max/2000/1*hUmRcqAz9_M2GZrY-F1TtA.png)
2. How can the server be assured a message was properly received?
- by reseving a responce from client side 
3. What classic design pattern is best represented by event driven programming?
- observer pattern 
4. How do you test an event driven system?
- with Unit Tests 



### Document the following Vocabulary Terms

**FIFO Queue**
- FIFO is an abbreviation for first in, first out. It is a method for handling data structures where the first element is processed first and the newest element is processed last


**Pub/Sub**
- Pub/Sub allows services to communicate asynchronously, with latencies on the order of 100 milliseconds.

- Pub/Sub is used for streaming analytics and data integration pipelines to ingest and distribute data. It is equally effective as messaging-oriented middleware for service integration or as a queue to parallelize tasks.

- Pub/Sub enables you to create systems of event producers and consumers, called publishers and subscribers. Publishers communicate with subscribers asynchronously by broadcasting events, rather than by synchronous remote procedure calls (RPCs).

### AWS SNS and SQS

## Use Cases

**Choose SNS if:**
- You would like to be able to publish and consume batches of messages.
- You would like to allow same message to be processed in multiple ways.
- Multiple subscribers are needed.

**Choose SQS if:**
- You need a simple queue with no particular additional requirements.
- Decoupling two applications and allowing parallel asynchronous processing.
- Only one subscriber is needed.