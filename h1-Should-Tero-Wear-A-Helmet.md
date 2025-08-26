# h1- Should Tero Wear A Helmet

# Threat Modelling

## Braiterman et al 2020: Threat modeling manifesto

There are four key questions and these are: What are we working on?, what can go wrong, what are we going to do about it and did we do a good enough job.

Firstly focus on protect to important assets.

Continuous and collaborative process.

## Shostack 2022: Welcome to the Worlds Shortest Threat Modeling Course

Uses the same four key question method as I mentioned on Braiterman.

Simple diagrams helps.

Threat modeling should be repaiting a lot.

## OWASP CheatSheets Series Team 2021: Threat Modeling Cheat Sheet
 Breaks the threat modeling to four steps: System or application decomposition, threat identification and ranking, defining mitigations, review and validation.
 
 Emphasizes understanding the system via data flow diagrams.

 # Infosec Scene
 ## Darknet dairies Episode
 I listened to Episode 42: Mini stories vol 2:
 
 I listened this episode because there was more then one stories but the most exciting one for me was pen tester trying and failing to sneak into a data center.

# a) Security Hygiene: 
## a1)What basic security practices should everyone follow?

Use unique and strong passwords,  use two-factor authenticator on your accounts, use antivirus programs to protect your devices, maybe you can enable find my device through your device for any chances of losing the device and most importantly (at least for me) be careful with emails. Because these mails could carry a virus that easily get in to your computer with one click

## a2)Are there some security hygiene practicies that every company or average Joe should follow?

For companies there are a lot of things but these are the most important ones in my opinion. Keep your antivirus and other softwares updated all the time, give lessons to employees about security awareness, backup your data and things are important for company, encrypt companie's sensitive data and monitor unusual activities like logging in a suspicious device.

# b)Make-belief boogie-man - a threat model for imaginary company.

Lets say company's name Kaan Büfe. It's a restaurant also provides online food order and delivery for people.

## b1) Key Assets:
 Crown Jewels: 
  
  Customer's personal information like their adress and name
  
  Espacially payment system
 
  Important but not as Crown Jewels:
 
  Website
  
  System for couriers

Website, customer service with a chatbot and delivery tracking system is the touchpoints for our customers. We have to serve the customer with a safe and easy system to make their order more easier and we also have to keep our system secured. If we dont make it probably customers gonna lose their trust to us and wont make orders in the future from us.

Diagram: Customers ---> Webpage or App ------> Payment ------>Bank 
                             |
                             |
                             V
                    Order System -----> Courier System

## b2) What can go wrong?
  Risks: 
   Denial of Service: There could be bot attacks to the server of the web page. Because of that customers cant give any orders and we cant make many because of that
  
   Information Disclosure: Customer addresses and payment details could be leaked and if it happens we would lose the trust of our costumers and it would affect us bad.
         
   Spoofing: If any authorized person's login informations got stolen by the hacker he can use this to trick the customers for to reach their important informations.
  Priorize biggest risks:
  
   High İmpact risks:
      
   Data breach of customer information.
   
   Payment fraud and this thing would lose money to us like hell.
   
   Medium İmpact risks:
   
   Courier system's manipulation and it could lead to couriers go to wrong addresses for orders.
   
   Personal misuse.
   
   Threat Actors probly would be cybercriminals who seeks money from customer information and the other things and I am not sure but could be the insiders cause there could be corrupted people inside of us to lose money to our company.

  ## b3) What are we going to do about it?
  I will use the META method to help my company about it.
   Mitigate: I would firstly enforce my employees to use MFA. Then I would start monitoring the loggings, having a good DDoS protection and I would use a firewall for my webpage.
   
   Eliminate: I would always delete the old versions of our apps after a new update fo the app and I would also delete all unused employee and admin accounts.
   
   Transfer: I would use buy a cyber insurance for the data breaches.
   
   Accept: Decide that the risks are on the lowest levet.

  # b4) Did we do a good enough job?
     I guess in cyber security its never enough but for now as I said before we did well but I would still make security test on my systems and probably keep my threat modelling updated.
