## Kringle Kiosk 
challenge=shell
```
Welcome to our castle, we're so glad to have you with us!
Come and browse the kiosk; though our app's a bit suspicious.
Poke around, try running bash, please try to come discover,
Need our devs who made our app pull/patch to help recover?
Escape the menu by launching /bin/bash
Press enter to continue...

~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Welcome to the North Pole!
~~~~~~~~~~~~~~~~~~~~~~~~~~~~
1. Map
2. Code of Conduct and Terms of Use
3. Directory
4. Print Name Badge
5. Exit
Please select an item from the menu by entering a single number.
Anything else might have ... unintended consequences.
Enter choice [1 - 5] 1

 __       _    --------------                                                
|__)_  _ (_   | NetWars Room |                                               
| \(_)(_)|    |              |                                               
              |            * |                                               
               --------------                                                
                                                                             
__  __                              __  __                                   
 _)|_                                _)|_          -------                   
/__|        Tracks                  __)|          |Balcony|                  
            1 2 3 4 5 6 7                          -------                   
 -------    -------------                             |                      
|Speaker|--| Talks Lobby |                        --------                   
|Unprep |  |             |                       |Santa's |                  
 -------    ------       |                       |Office  |                  
                  |      |                        --    --                   
                  |     *|                          |  |                     
                   ------                           |   ---                  
                                                    |    * |                 
    __                                               ------                  
 /||_                                                                        
  ||                                          __ __           --------       
  --------------------------              /| |_ |_           |Wrapping|      
 |        Courtyard         |              |.__)|            |  Room  |      
  --------------------------                                  --------       
    |                    |                                       |           
 ------    --------    ------                          ---    --------       
|Dining|--|Kitchen |--|Great |                            |--|Workshop|      
|      |   --------   |      |                            |  |        |      
| Room |--|      * |--| Room |                            |  |        |      
|      |  |Entryway|  |      |                            |  |        |      
 ------    --------    ------                             |  |        |      
               |                                             | *      |      
           ----------                                         --------       
          |Front Lawn|       NOTE: * denotes Santavator                      
           ----------                                                        
           
Enter choice [1 - 5] 2
# KringleCon III and Holiday Hack Challenge Code of Conduct
1. Use the challenges here to have fun, explore, engage, and develop your cyber security s
kills!
2. Be kind! Feel free to encourage and help other players! Let Santa's elves (support@holi
dayhackchallenge.com) know if something seems off. Please be mindful that there are childr
en playing. Santa is watching!
3. Please don't post full answers publicly until the official contest ends on Monday, Janu
ary 4, 2021.
4. SANS Holiday Hack strives to create an atmosphere of learning, growth, and community. W
e value the participation and input, in this event and in the industry, of people of all g
enders, sexual identities, cultures, socioeconomic backgrounds, races, ethnicities, nation
alities, religions, and ages. Please support this atmosphere with respectful behavior and 
speech. This applies to all online interactions associated with KringleCon and the Holiday
 Hack Challenge, including game chat and discussions.
# KringleCon III and Holiday Hack Challenge Terms of Use
1. This service includes a "group chat" component. We cannot make any guarantees about the
 accuracy, quality, or age-appropriateness of chat messages.
2. All activity and interactions within Holiday Hack Challenge are monitored and recorded.
 We use this information to maintain an environment that is both safe and condusive to lea
rning.
3. Players should avoid engaging in techniques on any Holiday Hack Challenge server that m
ay negatively affect the server's operational status and/or availability.
4. Players must not attack Holiday Hack Challenge servers (*.holidayhackchallenge.com, *.k
ringlecon.com, etc.) unless otherwise directed. If you have any questions about target sco
pe, please email: support@holidayhackchallenge.com.
5. E-mail addresses collected will be used in accordance with the SANS Privacy Policy (htt
ps://www.sans.org/privacy/).

Enter choice [1 - 5] 3
Name:               Floor:      Room:
Bushy Evergreen     2           Talks Lobby
Sugarplum Mary      1           Courtyard
Sparkle Redberry    1           Castle Entry
Tangle Coalbox      1           Speaker UNPreparedness
Minty Candycane     1.5         Workshop
Alabaster Snowball  R           NetWars Room
Pepper Minstix                  Front Lawn
Holly Evergreen     1           Kitchen
Wunorse Openslae    R           NetWars Room
Shinny Upatree                  Front Lawn

Enter choice [1 - 5] 4
Enter your name (Please avoid special characters, they cause some weird errors)...Giga
 ______
< Giga >
 ------
  \
   \   \_\_    _/_/
    \      \__/
           (oo)\_______
           (__)\       )\/\
               ||----w |
               ||     ||

Enter choice [1 - 5] 4
Enter your name (Please avoid special characters, they cause some weird errors)...`/bin/ba
sh`
shinny@dcfb28bd9562:~$ 
shinny@dcfb28bd9562:~$ exit
exit
 _________________________________________
/ #####hhc:{"hash":                       \
| "xxx",            |
| "resourceId":                           |
| "yyy"} |
| ##### ___ _ / __| _ _ __ __ ___ ___ ___ |
| | | \__ \ | +| | / _| / _| / -_) (_-<   |
| (_-< |_| |___/ \_,_| \__|_ \__|_ \___|  |
| /__/_ /__/_ _(_)_                       |
| _|"""""|_|"""""|_|"""""|_|"""""|_|""""" |
| |_|"""""|_|"""""|_| """ |               |
| "`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0- |
| '"`-0-0-'"`-0-0-'"`-0-0-' Type 'exit'   |
\ to return to the menu.                  /
 -----------------------------------------
  \
   \   \_\_    _/_/
    \      \__/
           (oo)\_______
           (__)\       )\/\
               ||----w |
               ||     ||
```

/home/shinny/welcome.sh


## Investigate S3 Bucket
challenge=awsbucket
```
elf@12c5004bf984:~$ cat TIPS
# TIPS
- If you need an editor to create a file you can run nano (vim is also
  available).
- Everything you need to solve this challenge is provided in this terminal
  session.
  
elf@12c5004bf984:~$ cd bucket_finder/
elf@12c5004bf984:~/bucket_finder$ ls
README  bucket_finder.rb  wordlist
elf@12c5004bf984:~/bucket_finder$ cat README 
Bucket Finder
=============

Copyright(c) 2011, Robin Wood <robin@digininja.org>

This project goes alongside my blog post "Whats In Amazon's Buckets?"
http://www.digininja.org/blog/whats_in_amazons_buckets.php , read through that
for more information on what is going on behind the scenes.

This is a fairly simple tool to run, all it requires is a wordlist and it will
go off and check each word to see if that bucket name exists in the Amazon's
S3 system. Any that it finds it will check to see if the bucket is public,
private or a redirect.

Public buckets are checked for directory indexing being enabled, if it is then
all files listed will be checked using HEAD to see if they are public or private.
Redirects are followed and the final destination checked. All this is reported
on so you can later go through and analyse what has been found.

Version
=======
1.0 - Release
1.1 - Added logging to file

Installation
============
I don't think it needs anything more than the built in modules so you shouldn't
need to install any gems. Just grab the file, make it executable and run it.

I've tested it in Ruby 1.8.7 and 1.9.1 so there should be no problems with versions.

Usage
=====
elf@12c5004bf984:~/bucket_finder$  
elf@12c5004bf984:~/bucket_finder$ cat README
Bucket Finder
=============

Copyright(c) 2011, Robin Wood <robin@digininja.org>

This project goes alongside my blog post "Whats In Amazon's Buckets?"
http://www.digininja.org/blog/whats_in_amazons_buckets.php , read through that
for more information on what is going on behind the scenes.

This is a fairly simple tool to run, all it requires is a wordlist and it will
go off and check each word to see if that bucket name exists in the Amazon's
S3 system. Any that it finds it will check to see if the bucket is public,
private or a redirect.

Public buckets are checked for directory indexing being enabled, if it is then
all files listed will be checked using HEAD to see if they are public or private.
Redirects are followed and the final destination checked. All this is reported
on so you can later go through and analyse what has been found.

Version
=======
1.0 - Release
1.1 - Added logging to file

Installation
============
I don't think it needs anything more than the built in modules so you shouldn't
need to install any gems. Just grab the file, make it executable and run it.
I've tested it in Ruby 1.8.7 and 1.9.1 so there should be no problems with versions.
Usage
=====
Basic usage is simple, just start it with a wordlist:
./bucket_finder.rb my_words
and it will go off and do your bidding.
You can specify which region you want to run the initial check against by using
the --region parameter:
./bucket_finder.rb --region ie my_words
The script will follow all redirects anyway so even if left at default, US Standard,
everything will be found that can be found but if most of the buckets you are
finding are in a different region then you'll be doing a lot of redirects so doubling
your network traffic.
You can also specify the --download option to download all public files found. Be
careful with this as there are a lot of large files out there. I'd personally do
the general search then only use this option with a select subset of bucket names:
./bucket_finder.rb --download --region ie my_words
The files are downloaded into a folder with the bucket name and then the appropriate
structure from the bucket. 
As some people are having trouble piping the output to files or other apps I've added
a logging option to send all output to a file. To use this just use the --log-file 
parameter:
./bucket_finder.rb --log-file bucket.out my_words
Licence
=======
This project released under the Creative Commons Attribution-Share Alike 2.0
UK: England & Wales
( http://creativecommons.org/licenses/by-sa/2.0/uk/ )
```
