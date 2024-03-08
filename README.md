# LLM Deployment FrameWorks

# Use Cases
## RealTime
1. Text to Text <br />
   In this type of applications we will interact with the LLM in realtime, there could be various types of deployment under this.
   - WebSockets - To interact with the chatbots websocket APIs will be better option to reduce latency between messages. 
   - WebRTC - To increase security on WebSockets.
   - Langchain - ConversationBufferMemory, ConversationChain, ConversationBuffer, ConversationMemoryBuffer - These can be used behind WebSocket to chat with LLM. <br />
2. Speech to Text <br />
   Here there are 2 application of speech to text, transcribing the text and speaker diarization. Both can be merged together too. There could be another application where after transcribing the use of LLM can be done to understand the text. 
   - WebSockets - One speaker channel will be involved and transcribing will be done in realtime. 
3. Speech to Speech <br />
   In this system there is a transcribing service as well as a LLM to generate the output followed by a text to speech model to convert the LLM text. Another option could be translating the speech and giving output in the required speech.
   - WebSockets - Single User
   - WebRTC - Multiple Users, typically like Zoom application.


## Async File Processing
1. Text to Text <br />
   In cases of Retrival Augmented Generation (RAG) we need to give system sometime to process the files given in the APIs. Hence we need the capacity of keeping async file processing in this case, so that the task is done on the background and the http port is closed for security issues.
   - Message Queing
2. Speech to Text <br />


# Technology Requirements
## Realtime System
1. Kafka
2. SQL DB
3. NoSQL DB
4. Vector DB
5. GraphQL (if required)
6. Docker
7. Kubernetes
8. Promethus
9. Graphana
10. Cloud Platform

## Async System
1. Rabbit MQ
2. SQL DB
3. NoSQL DB
4. VectorDB
5. GraphQL (if required)
6. Docker
7. Kubernetes
8. Promethus
9. Graphana
10. Cloud Platform
