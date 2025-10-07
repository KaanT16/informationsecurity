#h1 x) Read or watch and summarize

#h2 2.3 One-Way Functions

- One way functions are something that easy to apply or do but its really hard to reverse it.

- These functions are the core idea behind cryptography and they keep data safe because even if someone sees the result, they can’t easily figure out how it was made.

- They are used in a lot of areas like password checking, digital signatures and more.

- The main idea here is  there’s no fast or practical way to reverse the function and find the original input.

#h2 One-Way Hash Functions

- One way hash function takes the data and turns it into a fixed size "fingerprint" called hash.

- There are 3 important properties:

 - 1. One way: You cant get the original data back from the hash.

 - 2. Collision resistance: It's really hard to find two different messages with the same hash.

 - 3. Avalanche effect: If you change even one small part of the input it compeletly changes the result.

- Hash functions mostly used for storing passwords, checking data intergrity and digital signatures.

- Some examples are MD5, SHA-1, and SHA-256.

#h2 a) Install Hashcat. Test it with a sample hash.

 I used "sudo apt-get update" to update my pc and then used "sudo apt-get -y install hashid hashcat wget" to install the program. Then I created a file and got a big dictianory named rockyou. Then I opened and checked it if its working and yeah it was so then I moved to testing.
 
<img width="1273" height="895" alt="inffo7" src="https://github.com/user-attachments/assets/2134e657-5dde-4d6c-ac50-5d5c9ddd06a1" />

In the end I got the answer and the password was summer.

#h2 b) Crack this hash: d595b2086532422bbe654bc07ea030df

I went to the file on cmd and started doing the same things on the previous exercise. Then I used " hashcat-m O 'd595b2086532422bbe654bc07ea030df' rockyou.txt -o solved and it started to cracking the password and in few seconds I got the password and it was disobey
<img width="1275" height="887" alt="info2" src="https://github.com/user-attachments/assets/f5264e8c-d557-4d93-913f-875f80e66cd1" />
