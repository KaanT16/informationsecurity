#h1 Kill Chain Homework

#h1 x) x) Read and summarize.

#h2 Here is the summarization about Abstract:

- Conventional network defense tools such as intrusion detection systems and anti-virus focus on the vulnerability and assume succesfull intrusion, making them not enough againist sophisticated actors such as APTs.

- As I read this document focuses on intorducing intelligence - driven computer network defence(CND): a continuous, threat-centric risk management strategy that incorporates adversary analysis (capabilities, objectives, patterns) to reduce attacker success rates over time.

#h2 Section 3.2: Instrusition Kill Chain:

- The instrusion kill chain is adapted from U.S millitary targeting doctrine(F2T2EA) and concepts it as a instrusion multi-stage process and each step has to be completed for attack to be succesfull.

The seven defined stages are these ones:

1. Reconnaissance: Making research and selecting targets.

2. Weaponization: Creating a deliverable virus, trojan or something like that can give us remote access.

3. Delivery: Transfering the weapon to the target

4. Exploitation: Execution of the virus or trojan to exploit a vulnerability in the target system.

5. Installation: Establishment of persistent access via malware/backdoors.

6. Command and Control: Enabling remote access and ongoing control of the compromised system.

7. Actions on Objectives: Carrying out the main mission.

- By aligning each stage with defensive options defenders can interrupt or delay attacks at any stage and even could break the attack and could prevent the attacker from his mission.

#h2 My insight/question:

My only question about this whole tactics are which defending ways are more practical and more effective against the attackers?

#h1 a) Tactics, tools and procedures:

#h2 Tactic:

- The reason of the adversary's technical goal during attack

- For example Persistence: Ensuring contuniued access to system even after reboots or credential changes.

#h2 Technique:

- Definition: The how a general method adversaries use to achieve a tactic.

- For example Creating Account: Adversaries may create new local or domain accounts to maintain access

#h3 Subtechnique:

- Definition: A more specific implementation of a technique.

- For example Local Account: Adversary creates a local account on a machine for persistence.

  #h4 Procedure:

- Definition: The exact, real-world implementation of a technique or subtechnique, often observed in threat reports.

- For example APT29: APT29 has been observed creating hidden local administrator accounts using PowerShell scripts to maintain persistence in victim environments.
