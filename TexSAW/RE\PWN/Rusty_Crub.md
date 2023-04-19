# Rusty Crub
- Solves - 35
- Points - 200
#
# Description
You are given a rust binary. Give the proper key to obtain the flag! But beware, Rust is not the same as C.

# Attachments
[Файл crab](./sources/crab)
# Solution
A lyrical digression. I hate to reverse Rust.

I don't know how we had to figure out what we were getting in the disassembler, I just used grep on the keyword and got a base64 string, which turned out to be a flag.

Note: always run the binary through strings and grep. This might help to solve the task quickly.
