# Line-based-TCP-client-server

There are two applications in this project - one that acts as a server and another that acts as a client. 
The protocol is TCP, and on the application-level, the protocol is a simple character-based protocol. A simple character-based protocol is just using standard ASCII characters, i.e. CHAR. 
we start to implement the client and once the client works, we implement the server. The server is only required to handle ONE client at a time. But multiple clients should be able to queue up for service. 
If the client accepts ANY of the protocols, it has to respond with 'OK\n'. If it does not, then it should disconnect. 
In the next stage, the client is to read a string that is randomized at the server. The string is constructed from three parts; '<OPERATION> <VALUE1> <VALUE2>\n'.

OPERATIONS are; 

add/div/mul/sub for these VALUE1 and VALUE2 have to be integers. 
fadd/fdiv/fmul/fsub for these VALUE1 and VALUE2 are floatinpoint values. 
  
  The server reads this and compares it with its result, if they match the server sends back a string with 'OK\n', otherwise 'ERROR\n'.
