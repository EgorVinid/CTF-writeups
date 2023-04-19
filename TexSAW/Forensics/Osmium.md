# Osmium
- Solves - 45
- Points - 100
#
# Description
Hey I've gotten this rock, but I don't know what I can get out of it. 
It's pretty heavy, and apparently it's made out of Osmium, I was told. See if you can extract anything out of it for me.<br>
HINT: 
This rock has been sitting under huge amounts of pressure for a pretty long time. 
It seems highly compressed and contaminated with a bunch of tar and slags too. 
There doesn't seem to be any regular pattern to the tar contamination and compression that it experienced though...

# Attachments
[Файл rock.rock](./sources/rock.rock)
# Solution
In general, this was a fairly typical task, but with one change - the file rock.rock is actually a zip archive (which you can check through Hex editor) and in this file there is the same archive and a text file slack.txt. All you had to do in this assignment was to write a script that unpacked the attached zip archives and extract the flag.txt file from the last one.

Here's a sample script

```python

import os, zipfile

for i in range(0, 1000):
    if i!=0:
        os.rename(f'rock.rock', f'rock{i}.zip')
    zipfile.ZipFile(f'rock{i}.zip').extractall()
```

