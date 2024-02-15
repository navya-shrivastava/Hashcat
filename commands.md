# Commands

## The following commands were run by us on the terminal to show the different types of attacks supported by Hashcat

### Dictionary Attack
hashcat -m0 -a0 hashedPass.txt rockyou.txt —-show

### Combination Attack
hashcat -a1 -m0 hashed.txt wordlist1.txt wordlist2.txt

### Brute Force Attack (without mask)
hashcat -a3 -m0 hashed.txt

### Brute Force Attack (with mask)
hashcat -a3 -m0 hashed.txt ?d?d?d?s?d?d?d

### Mask Attack
hashcat -a6 -m0 hashed.txt wordlist1.txt ?d?d?d

### Rule-based Attack
hashcat -a0 -m0 -r ..\hashcat-6.2.6\rules\best64.rule hashed.txt wordlist1.txt
