# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.
## PROGRAM
## Name: NIRANJAN S
## Reg No:212224040221
## Client:
```
import socket 
s=socket.socket() 
s.connect(('localhost',8000)) 
while True:
    msg=input("Client > ") 
    s.send(msg.encode()) 
    print("Server > ",s.recv(1024).decode())
```
## Server:
 ```
import socket 
s=socket.socket() 
s.bind(('localhost',8000)) 
s.listen(5) 
c,addr=s.accept() 
while True: 
    ClientMessage=c.recv(1024).decode() 
    c.send(ClientMessage.encode())
```
## OUTPUT
## CLIENT........................................................................... SERVER.................................................................
![427927378-9b55e2ed-d483-4d5e-ae32-e1a611ddcc40](https://github.com/user-attachments/assets/43b02dd6-fcb2-4902-b173-145704662213)


## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
