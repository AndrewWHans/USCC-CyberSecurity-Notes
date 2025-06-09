# Lab commands used in the Linux Command Line, with Q/A's
Q: How do we look for files that contain a particular string? <br>
grep -rl sockaddr_in /usr/include

**to get the matches:** grep -rl sockaddr_in /usr/include | wc -l <br>
30

Q: How many files in the pictures dir?
ls Targets/Pictures/ -> **gives you all the columns of what is within the dir, but if you did:** <br>
ls Targets/Pictures/ | wc -l -> **give you the n# of files**

# Other Commands used with explanations

ls Targets/Pictures/ | cut -d. -f2 | head

lab@LAB:~/Exercises$ md5sum Targets/Pictures/* |awk '{print $1}' | sort | uniq -c

lab@LAB:~/Exercises$ ps -ef | tail -n +2 | head

lab@LAB:~/Exercises$ ps -ef | tail -n +2 | awk '{print $1}' | sort | uniq -c

tail allows to start counting by the beginning of the file, 

lab@LAB:~/Exercises$ ls -l $(grep -irl mail /etc 2>/dev/null)

lab@LAB:~/Exercises$ grep -wf <(cut -d: -f3 Targets/passwd | sort | uniq -d) Targets/passwd
