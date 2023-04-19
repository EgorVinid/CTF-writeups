# A Prime Problem 
- Solves - 15
- Points - 400
#
# Description
Suppose I generate primes p and q for RSA in the following way:

Choose a random 2048 bit integer
p is next prime after that integer
Choose another random integer r where 0 < r ≤ 2^1023
q is next prime after r + p
n = p*q Can you factor n and recover the flag?

Hint: CVE-2022-26320
# Attachments
[Файл public.pem](./sources/public.pem)
[Файл key_gen_flag.bin](./sources/key_gen_flag.bin)
# Solution
Решение
