# neural-network-multiclass-classification
classify network attacks with neural network

**Features**
<br>The dataset has a total of 41 features, but I only used the following:
1. duration: how long connection lasted
2. src_bytes: Number of data bytes transferred from source to destination in single connection
3. dst_bytes: Number of data bytes transferred from destination to source in single connection
4. num_file_creations: Number of file creation operations in the connection
5. num_shells: Number of shell prompts
6. num_failed_logins: Count of failed login attempts
7. wrong_fragment: Total number of wrong fragments in this connection
8. urgent: Number of urgent packets in this connection. Urgent packets are packets with the urgent bit Activated
9. is_guest_login: 1 if the login is a ``guest'' login; 0 otherwise
10. su_attempted: 1 if ``su root'' command attempted or used; 0 otherwise
11. land: if source and destination IP addresses and port numbers are equal then, this variable takes value 1 else 0

**Target**
<br> Dataset originally contained 23 different attack classifications (ex. sql attack, buffer overflow, httptunnel, etc). 
<br>To to simplify the problem, 
they were categorized into the following generic types:
1. DOS: denial of service; disrupts service and makes it temporarily unavailable
2. Probing: scan a system/network to check for vulnerabilities
3. U2R: User to root, getting root access
4. R2L: Remote to local, obtaining access to victims system or network
5. Normal
