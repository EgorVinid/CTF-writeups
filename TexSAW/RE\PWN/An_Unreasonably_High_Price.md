# An Unreasonably High Price
- Solves - 46
- Points - 100
#
# Description
You are given an executable binary that, when run, will open up a pawn shop with a flag for sale. Correctly guessing the flag's price will give you the flag for free. Decompile the binary to figure out the value of the price.

nc 18.216.238.24 1500

# Attachments
[Файл shop](./sources/shop)
# Solution
By disassembling the binary, we see a large number of mathematical expressions whose result is compared with the value entered by the user. Just rewrite the code in any language you like (it may not work, better use C or C++) and enter the resulting value to take our flag
