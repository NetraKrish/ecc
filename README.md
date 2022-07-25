# ecc
ecc encrytpion for otp transfer
To begin, create a folder called "netra_secured_folder" and
store all of the files Server.cpp, Client.cpp, and FiniteFieldElement.hpp in
there.
• Open two terminals:
1. Server
2. Client
• Move into the directory called “pranav_saransh_secured_folder” in both
the terminals.
• Enter the following command in terminals
1. g++ server.cpp -o server
2. g++ client.cpp -o client
• The above command will compile both the server.cpp and client.cpp files
and will make the execution file for them.
• Next enter the following commands in the terminal
1. ./server -For server terminal
2. ./client -For client terminal
• Now both the C++ files will start its execution.
• Next enter the OTP in the server terminal.
• Start the client terminal and start listening from the server socket.
• The main working of the system is that the bank will enter the OTP. It will
encrypt the OTP using its private key and shared key between the bank
and the user and using the ECC algorithm. After that it will create a socket
and will send the encrypted message to the client (the user). After that
the user will read the message and decrypt the message using its private
key and shared key between the bank and the user. After that for the
authentication the user has to enter the OTP in the ATM. If he entered
wrong OTP authentication is failed else authentication success. Also, if an
eavesdropper is trying to get the encrypted message, he will expose
himself and the bank will be alerted as the data is being accessed by the
unauthorized person.
