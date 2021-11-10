# Read 14: Event Driven Architecture

1. What’s the difference between a FIFO and a standard queue?
 FIFO preserves the exact order in which mmessages are sent and received. Placing of sequencing information is not required.
 Standard queues attempt to preserve the order, but it's not guaranteed. [ref](https://aws.amazon.com/sqs/faqs/)
2. How can the server be assured a message was properly received?
   The message stays in the queue until the receiver takes action to delete it. Otherwise the message stays in the queue and can be requested again. The fact that the receiver moves to delete the message tells the server that it was received and processed.
3. What classic design pattern is best represented by event driven programming?
   Observer pattern
4. How do you test an event driven system?
   By logging the steps


## Vocabulary

- FIFO Queue - First in, first out queue. First message into the queue gets delivered first.
- Pub/Sub - Publishe/Subscribe system - messages are pushed to subscribers of a topic as and when they are sent by publishers. [ref](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)

## Resources

[AWS SNS and SQS](https://www.youtube.com/watch?v=mXk0MNjlO7A)



[**<== BACK**](401-toc.md)