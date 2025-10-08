# wargames-bandit-level-7-to-12
Hi this is my third time doing that i finished networkchuck guide on linux and python and now i try something else that regroup almost everything i learned even more so pls if you have any advice so i can be better again and again feel free to share it with me! 

---

the site where i trained is very famous in this world because it's **[wargames](https://overthewire.org/wargames/bandit/bandit0.html)** 


**[LEVEL 6 > 7](https://overthewire.org/wargames/bandit/bandit7.html) :**
for this level i did almost the same thing as the previous level so i just type this command `find / -type f -user bandit7 -group bandit6 -size 33c` you'll fdind a bunch of text all starting by **find:** execpt one
threre is you password after find it you just have to copy it then **cat** him : `cat /var/lib/dpkg/info/bandit7.password` the only thing that change from the previous one is that you have to find a group and that 
i changed the **dot .** for the **slash /** why ? because i was in the root and when i typed `ls` nothing appear i'd to add ` -al` to see something and then i saaw i was in the root so i started my command with
`find /` and not `find .` 

**[LEVEL 7 > 8](https://overthewire.org/wargames/bandit/bandit8.html) :**
easy level you spawn they tell you you have to find the password and it's next to the word **millionth** in the data.txt file. it the first time we using it in this series but the command's very known about all of us wich is `grep`
this is the only file here and the full command was `cat data.txt | grep millionth` great job you finish level 7 > 8 now let's go to the end!

**[LEVEL 8 > 9](https://overthewire.org/wargames/bandit/bandit9.html) :**
in this level i was a little lost i first because i had to read some commands the one that seems correct for this exercice thanks to the **commands you may need to solve this level** section that's very helpful 
whatever go focus. so for thisd exercice you have another data.txt file and inside a loooooooooot of password but they also tell you that all of them except 1 appear several times, the 2 commands that keep my attention
and that'll be used are `[sort](https://manpages.ubuntu.com/manpages/jammy/en/man1/sort.1.html)` and `[uniq](https://manpages.ubuntu.com/manpages/jammy/en/man1/uniq.1posix.html)`. i let you here the full explanation of these command here 
and now the command is wait just for uniq i add `-c` so when they are listed i have a number on the side that shows me how many of these code there is so the command is `sort data.txt | uniq -c` and now i just have to 
look for the password where it has only one appearance

**[LEVEL 9 > 10](https://overthewire.org/wargames/bandit/bandit10.html) :**
thanks for the time reading just before it save me a lot of time for this one that was very simple to do. so same thing we have a data.txt but inside it you have a lot of alian text and you can't even see all of it so you have to strings that up
by doing `strings data.txt` if you learn a little bit of python you'll understand very easily that it sort you only the human readable text and then you can already search for the password but if you want to do it the right way you have to
add the `grep` command and do `strings data.txt | grep "=="` and my bad i forgot to tell you but i hope you have read the exercice and not cheatin without learning but thwe password is preceded by several "=" characters

**[LEVEL 10 > 11](https://overthewire.org/wargames/bandit/bandit11.html) :**
well i didn't know the command but very standart as cyber is in the beginning. i don't want to loose time sorry but the command is simple the code is encoded in base 64 so y ou have to ????.... decode him with base64 that's the right anwser gg so just do 
`base64 -d data.txt` (the -d is for decode) now let's go for the golden last!

**[LEVEL 11 > 12](https://overthewire.org/wargames/bandit/bandit12.html) :**
this one was fun for being the last so i will stop there. to finsh it you have a data.txt file and when you `cat` him you have a weird word and a password but it's told to you that the password has been rotate 13 times ?? so i don't even really
understand because i'm a noob in this game but with my cyber logic i jump on the firefox copy the text before and write **rotate13 decoder** i click on it put my text and it show me the right code with the word the password is and so on 
i don't even know how that works but i will read about that for sure it's so much amazing  

well well well it seems to be the end for today but don't worry we'll find us tomorrow for sure!!
so goodbye and always be positive it's important and call your family too it's important and don't cost much!




