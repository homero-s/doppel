# Doppel 3b1b talent page phishing puzzle

If we start off by assuming that the attacher does not already have access to company systems, (if they did then why are they sending phishing emails) then there is no way for the attacker to know:

- The baseline distribution **q** representing natural phrase frequencies that the company is using
- The fact that the email detector is using KL Divergence to detect suspicious emails
- The constant **C** above which an email is flagged

In order to find the optimal distribution **p** he attacker would have to first find their own baseline distribution **q** presumably from a public corpus of the english language. Start off by having **p=q** then incrementally increase the probablilty of using a specific phrase untill the payoff **s** drops to zero. Then keep using the probability that had the max payoff. 

In other words an attacker would have to empirically determine the optimal distribution because they are working blindly. 
