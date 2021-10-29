# HW_ASGMT

<h1>Goal</h1>

The goal of this assignment was to complete the challenges and lessons in the Labex course "[Linux for Noobs](https://labex.io/courses/linux-for-noobs)." During this challenge, we were specified to document the steps down to complete each challenge.

<h3>Challenge 1</h3>

• Used sudo adduser for jack and for bob account creation

• Used sudo groupadd for dev and test group
Used sudo usermod -a -G to add users to respective groups. Must have -a flag or it will just mod
instead of add.

Used sudo vi /etc/passwd, followed by I for edit mode, to edit the user’s default shell. ESC to
end mode and ZZ to save + quit command.

<h3>Challenge 2</h3>

• Used sudo su, followed by find /etc -name *list

• Utilized ownership change through sudo chown labex source.list

• Changed the file access using chmod to 700 for source.list

<h3>Challenge 3</h3>

First googled the date command function parameter usage because man is hard to read. Want to use
date as a variable.

Created folder using mkdir tmp .

Var log is system level, so sudo needed.

Used the command tar -cjvf ./tmp/$(date “+Y%-%m-%d”).tgz /var/log to create compressed zip with output name of the current date of the var log folder to the temp folder.


<h3>Challenge 5</h3>

Pulled data using the wget command.

For mail, I used grep @ data to grab all lines with a @ in it because after using cat to view the content, it
didn’t show any complex patterns that required multiple parameters. For the opposite you can do grep -
v “@” data2 .

For Num, I used ^ in the beginning along with [0-9], so it looks like grep ^[0-9] data2 . This searches for
all lines with a range of 0-9 as the first character and prints them out. The assignment did not ask for
exclusions such as emails.

Last, I used > “file” to print to file
