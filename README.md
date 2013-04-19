Mytube
======

This set of 3 files seeks updates on channel you decided and download the last videos.
There is also the last version of youtube-dl (http://rg3.github.io/youtube-dl/)

Prerequisite
====
* CURL
(apt-get install curl)
That's it!
* Linux
* A smb/nfs file share or an web server where you can access this file

Installation
====
Copy the files on any directory you want.
(you should have access to the file on your computer either from a browser or a file share)

Usage
====
Just create a channel you want to query (Every 5 minutes)

create_channel $username

You have to get the username from the youtube channel
Ex: http://www.youtube.com/user/joueurdugrenier

--> create_channel joueurdugrenier

It will then create a directory with an index.html

Troubleshooting
====
As for now, the scripts should be consider alpha, anyway it works great for me.
Still it is really advice to NOT USE IT ON A SERVER WITH CRITICAL APPLICATIONS.

if anything bad happens it will

--> Create unwanted cron action (repeat every 5 minutes) (beware if you received email from cron it will be
considered as spam)
To resolve this check your cron with crontab -e

--> Create unwanted file in the current directory

--> Filled up your space : Create a LOTS of videos files (nothing will be erased so you should be aware of this)

--> Create bogus index.html






