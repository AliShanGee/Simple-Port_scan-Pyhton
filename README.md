# Simple-Port_scan-Pyhton
My first project in cyber_security to 80 number port scanner create simple port scanner in python
import socket #use socket module to create tcp connection
host_ip = input("enter your ip") #input your ip address
host_port = 80 #scan 80 number port 
sock = socket.socket() #use socket module
try:
    sock.connect((host_ip,host_port)) #create connection 
    print("[+]port is open") #if connect successful than print this
except:
    print("[-]port is closed") #id does not create successful connect than print this
