# port-scanner-and-recorder
Basic python Port scanner


import socket
import sys
sys.stdout = open('log.txt', 'w')
print("Write this to file.")

s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)

target = input("Enter a ip to scan: ")

def pscan(port):
    try:
        con = s.connect((target,port))
        return True
    except:
        return False

for x in range(25):
    if pscan(x):
        print(ƒ,"Port {x} is open")

import sys
sys.stdout = open('log.txt', 'w')
print("Write this to file.")
