# What is there to hide?
- Solves - 33
- Points - 100
#
# Description
Your mission is to decrypt this intercepted message to solve the challenge.

nc 18.216.238.24 1013

Hint: Fine. I'll give you the function I used to encrypt it, can you come up with the decryption function?
![encrypt](./sources/encryptFunc.png)
# Attachments

# Solution
The original incarnation of the standard one time pad. 

The key is in base64 format, so you must first decode it.

Let's write a decryption function and pass the key and the ciphertext into itэ

```python
def decrypt(encrypted_message, key):
    encrypted_ints = [ord(i) for i in encrypted_message]
    key_ints = [ord(i) for i in key]
    decrypted_ints = [(((e-65-k+65)%26)+65) if e in range(65,91) else (((e-97-k+97)%26)+97) if e in range(97,123) else e for e,k in zip (encrypted_ints,key_ints)]
    decrypted_str = [chr(i) for i in decrypted_ints]
    return ''.join(decrypted_str)

print(decrypt('Hn vgkq gnsb nimt gpr ompvr', 'LjiPmsxFTnODzFTOcDTiTmYyEkU'))

output - We must take over the world
```
