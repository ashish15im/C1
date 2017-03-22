# C1
C port Scanner
The current port scanner works on by trying to establish a connection with every port that is to be scanned and make sure the port is
open or closed it is not stealthy but it can do the job.
It involves in a three way hand shake between 2-hosts hence it consumes maximum time to finish the job.
Local system ----&gt; sends tcp syn packet -----&gt; Remote system
Local system &lt;---- replies with a syn+ack packet &lt;----- Remote system
Local system ----&gt; sends ack packet -----&gt; Remote system
First compile the program using gcc. Its simple.

# gcc portscanner.c
Now run the program and provide the necessary input

# ./a.out
Enter hostname or IP : google.com

Enter start port number : 75
Enter end port number : 85
Doing gethostbyname…Done
Starting the portscan loop :
80 open
#
So the above program scanned ports 75 to 85 on google.com and found only port 80 to be open, which is the webserver port.
