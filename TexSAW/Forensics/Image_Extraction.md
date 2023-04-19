# Image Extraction
- Solves - 21
- Points - 150
#
# Description
Uncover a jpg file from the given file. The flag is in that image.<br>
HINT: Look at the hex!

# Attachments
[Файл Challenge.pdf](./sources/Challenge.pdf)
# Solution
We are given a PDF file that does not open. We look in the HEX via Hex-editor and notice the signature bytes 'PK', which tells us that it is actually a zip file. But at the beginning of the file there are FF D8 bytes, which are the signatures for the JPG file. Let's replace them with the corresponding zip file signatures and open the archive in peace. It contains a picture with the cat, on which the codes of the flag symbols are written
