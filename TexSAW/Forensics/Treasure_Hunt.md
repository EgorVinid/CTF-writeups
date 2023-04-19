# Treasure Hunt
- Solves - 41
- Points - 150
#
# Description
Find the flag hidden deep within the treasure.
Welcome to the Clash Royale Treasure Hunt. 

The order of chests goes silver, gold, and then magical. 

Open (crack) each chest to find cards (passwords) that may help you. 

Happy clashing! 

# Attachments
[Файл SilverChest.jpg](./sources/SilverChest.jpg)<br>
[Файл GoldenChest.jpg](./sources/GoldenChest.jpg)<br>
[Файл MagicalChest.jpg](./sources/MagicalChest.jpg)<br>
# Solution
Three pictures with chests are given. The first thing to do is to look through strings on the first picture. We'll get a password of some kind. Then we run the steghide utility with the obtained password and take out the txt file with the base64 string from the picture. After decoding we'll get the password for the second picture. We do the same with the third picture and get our flag.
