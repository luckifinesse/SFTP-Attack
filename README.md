# SFTP-Attack
A SFTP Brute Force Attack is a Python-based tool designed to perform dictionary attacks on SFTP servers. It systematically attempts various username and password combinations from a predefined list to capture valid login credentials.

# What is SFTP?
SFTP(Secure File Transfer Protocol), is a new and secure version of FTP(File Transfer Protocol). For transferring files between computers over a network we use SFTP. It provides a secure and encrypted connection, typically over SSH (Secure Shell), to protect data during transit. SFTP provide more security for file transfers compared to traditional FTP.

# What is dictionary attack?
A dictionary attack is a kind of hacking method in which an attacker uses a precompiled list of login credentials(username & passwords), called a “dictionary,” in an effort to repeatedly try and guess a large number of passwords in an attempt to obtain unauthorized access to a system or account. Typically, this list consists of dictionary terms, frequently used passwords, and password variants. Dictionary attacks depend on the possibility that the right password is among the entries in the selected dictionary, as opposed to brute force assaults, which attempt every conceivable combination.

# Installation for iha089ftp
iha089ftp is a tool written in Python language that is used to obtain the correct login credentials of an SFTP server using a dictionary attack. Now, let’s see how you clone and use the iha089ftp tool on your operating system.

If git is already setup on your system then you can easily clone iha089ftp using git

git clone https://github.com/luckifinesse/SFTP-Attack.git

After cloning/downloading it, go to iha089ftp directory.

Then run python install.py command which installs this tool on your system and after installation you can access iha089ftp from anywhere in the terminal by simply typing iha089ftp.

If you want to use it without installation you can run python start.py as usual. But this only works in the current directory so if you try to access it from anywhere you have to run python insatll.py first.

After installation, you just need to type iha089ftp on the terminal to launch it.

when launch then it will ask some information related to target and dictionaries.

Enter Remote server IP: This field asks for target IP. So, enter the target SFTP server IP Address.

Enter Remote server PORT: This field asks for target PORT. Basically SFTP or FTP use 21 port by default but in some case it will be change. So, enter target port on which SFTP server running.

Enter username wordlist: This field asks for the username dictonary. So, enter the username dictionary path here.

Enter password wordlist: This field asks for the password dictionary. So enter the password dictionary path here.

How many thread you create: This field requires a thread. Threads are mainly used to create multiple parallel processes. This improves the speed of password testing. So, use 10-30 threads (remember your system preferences)

After entering the above fields it starts the dictionary attack on the SFTP server by selecting the username and password from the dictionary one by one.

# Backdrow of dictionary attack:
Time consuming: Dictionary attacks require carefully attempting every password in the dictionary until the right one is discovered, which makes them time-consuming. The size of the dictionary and the difficulty of the passwords determine how long it takes. Longer and more complicated passwords might take a lot longer to figure out.

Ineffective against login limitations: Dictionary attacks are not certain to be effective since they depend on precompiled lists of passwords. The attack may not be successful in determining the target password if it is very unique or does not appear in the dictionary. This restriction stands in contrast to more thorough techniques such as brute force assaults, which attempt every conceivable combination.

Not guaranteed success: Ineffective against login restrictions: To stop or lessen dictionary attacks, a lot of servers and online services use security measures like account lockouts or login rate limits. The attacker could be locked out after a predetermined number of unsuccessful login attempts if there is a restriction on the amount of tries. This countermeasure guards against automated, quick-fire password guessing attempts and lessens the impact of dictionary assaults.
