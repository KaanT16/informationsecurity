#h1 x) Read and summarize 

#h2 Schneier 2015 – Applied Cryptography Ch.1 Foundations

- As I get it crypto means math methods for secure communication.

- Back in time there was different encryptinos named Ancient encryption (Caesar cipher, frequency analysis).

- As it mentioned Cryptography is divided into two main areas. First one is traditional symmetric encryption so in short same key. Second one is asymmetric encryption so in short public key + private key.

- Security of your messages also not just coming from encryption but protecting your keys.

- Cryptography alone is not enough; protocols, security models, and implementation errors also matter.

- Cryptography is also getting used for authentication and security protocols.

#h2 Karvinen 2023: PGP – Send Encrypted and Signed Message – GPG

- PGP and its open source version GPG explains how to easily encrypt messages.

- The basic idea: encrypt with the recipient’s public key → only the recipient’s private key can decrypt → ensures confidentiality.

  Typical Steps for setting it:

  1. Install GPG
 
  2. Generate a key pair.
 
  3. Import someones public key.
 
  4. Encrypt the message.
 
  5. Decrypt the message.
 
#h1 Install OpenSSH server, connect to it using 'ssh' client.

- I used sudo apt install openssh-server to install a server. Before that I also updated system.

- After that to be sure server installed I used sudo systemctl status ssh command to check and it said server is active.

- Then I used ssh kaan@myIpAddress to connect to server.

#h1 Automate SSH connection using public keys.

- Firstly I used ssh-keygen -t rsa to generate a key than selected the location for the keys.

- After that I copied public key to the server with the 'ssh-copy-id kaan@myIP' command.

- Then I just tried to connect by just typing 'ssh kaan@myIP' and it got me to connect to server without any authentication because of the key.

#h1 Password manager, open and cloudless. Choose a password manager that 1) works without cloud 2) is free, open source sofware. Install it. Demonstrate its use. Explain why a password manager is needed i.e. what kind of attacks or threats it protects against.

- Firsly I researched for a password manager and found keepassxc and installed it with the command of 'sudo apt install keepassxc'.

- First of all after the installation I made a database.

- After that I saved it and then made a new entry for youtube thanks to password manager.

- There are some reasons for the manager needed and these are basicilly these:

   -They auto-fill login forms only on trusted websites, reducing the risk of entering credentials on malicious sites. Thanks to that we can  prevent phishing attacks.

   - They generate and store unique passwords for each account, preventing the domino effect if one account is compromised.
 
   - They create strong, random passwords, enhancing security beyond simple or reused passwords.
 
#h1 Encrypt and decrypt a message with 'gnupg', using PGP public key cryptography.

- First of all I downloaded the gnupg by 'sudo apt install gnupg' command.

-  Then I use 'gpg --full-generate-key' to generate my key pair.

-  I generated it and sent it to my email.

- Then I used gpg --armor --export kaanturksan9912@gmail.com > mypubkey.asc to export my public key.

-  And I got stuck here dont know what to do unfortunetly.
