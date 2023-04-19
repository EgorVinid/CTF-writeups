# Ghost in the Clipboard
- Solves - 56
- Points - 250
#
# Description
A hacker has broken into your computer and stolen one of your passwords. 
You were able to extract the AppData folder as it was right after the attack took place. 
See if you can find out which password (the flag) they stole so you can change it before any damage is done.

You had clipboard history turned on in windows at the time of the attack. Perhaps the attacker copied the password? 

# Attachments
-----
# Solution
We are given an Appdata folder with some information inside and a prompt tells us the history of the keyboard.
Actually, I hardly solved the task the way I needed to, because I only ran this command in the terminal and got a flag.

`grep 'texsaw{' -r .`
