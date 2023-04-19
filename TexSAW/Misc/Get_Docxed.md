# Get Docxed
- Solves - 41
- Points - 150
#
# Description
My professor hid the answers to the final exam somewhere in this 2305_Syllabus_Spring2018.docx file. Can you find it?

Hint: Careful letting Word recover the contents of the document, it may delete the flag. If you think that happened to you, just re-download the file from here again.

# Attachments
[Файл 2305_Syllabus_Spring2018.docx](./sources/2305_Syllabus_Spring2018.docx)
# Solution
doc files are essentially archives, so just unzip this file and find an archive in it. But here's the problem - the archive is password protected. No problem, let's try to crack the password. The hashcat utility and the rockyou.txt wordlist will help us nicely. Having found the password, we unpack the archive and take out the text file with our flag. 
