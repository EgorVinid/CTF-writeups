# Dial Tones
- Solves - 30
- Points - 200
#
# Description
Can you believe Britney Spears released her iconic album "Oops!... I did it Again" all the way back in 2000? Feels just like yesterday. What other whacky hijinks were the youth up to back in the day?

You'll need to surround the final message with the flag format to submit: texsaw{message}

# Attachments
[Файл audio.wav](./sources/audio.wav)
# Solution
In General, this was one of the most interesting and original task, the admins thank you.

We are given an audio file, and after listening to it, we understand that it is the sound of typing on a push-button phone.

Next we have two options. We can manually match the frequency table to the keys being dialed. Or we can use a ready-made [solution](https://github.com/ribt/dtmf-decoder). 

Once we get the decoded button numbers, we run through a [T9 decoder](https://www.dcode.fr/t9-cipher) to get all the possible variations of the typed characters and take our flag.
