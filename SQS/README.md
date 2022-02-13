
## ReceiveMessageWaitTimeSeconds
minimize the number of empty responses from polling requests: When the ReceiveMessageWaitTimeSeconds property of a queue is set to a value greater than zero, long polling is in effect. Long polling reduces the number of empty responses by allowing Amazon SQS to wait until a message is available before sending a response to a ReceiveMessage request. 