## Kringle Kiosk
<details><summary>Click to expand</summary>

* [Conversation: Shinny Upatree](conversations.md#shinny-upatree)

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
1. Use the challenges here to have fun, explore, engage, and develop your cyber security skills!
2. Be kind! Feel free to encourage and help other players! Let Santa's elves (support@holidayhackchallenge.com) know if something seems off. Please be mindful that there are children playing. Santa is watching!
3. Please don't post full answers publicly until the official contest ends on Monday, January 4, 2021.
4. SANS Holiday Hack strives to create an atmosphere of learning, growth, and community. We value the participation and input, in this event and in the industry, of people of all genders, sexual identities, cultures, socioeconomic backgrounds, races, ethnicities, nationalities, religions, and ages. Please support this atmosphere with respectful behavior and speech. This applies to all online interactions associated with KringleCon and the Holiday Hack Challenge, including game chat and discussions.
# KringleCon III and Holiday Hack Challenge Terms of Use
1. This service includes a "group chat" component. We cannot make any guarantees about the accuracy, quality, or age-appropriateness of chat messages.
2. All activity and interactions within Holiday Hack Challenge are monitored and recorded. We use this information to maintain an environment that is both safe and condusive to learning.
3. Players should avoid engaging in techniques on any Holiday Hack Challenge server that may negatively affect the server's operational status and/or availability.
4. Players must not attack Holiday Hack Challenge servers (*.holidayhackchallenge.com, *.kringlecon.com, etc.) unless otherwise directed. If you have any questions about target scope, please email: support@holidayhackchallenge.com.
5. E-mail addresses collected will be used in accordance with the SANS Privacy Policy (https://www.sans.org/privacy/).

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

```

Solution:
```
Enter choice [1 - 5] 4
Enter your name (Please avoid special characters, they cause some weird errors)...hello;/bin/bash
 _______
< hello >
 -------
  \
   \   \_\_    _/_/
    \      \__/
           (oo)\_______
           (__)\       )\/\
               ||----w |
               ||     ||
   ___                                                      _    
  / __|   _  _     __      __      ___     ___     ___     | |   
  \__ \  | +| |   / _|    / _|    / -_)   (_-<    (_-<     |_|   
  |___/   \_,_|   \__|_   \__|_   \___|   /__/_   /__/_   _(_)_  
_|"""""|_|"""""|_|"""""|_|"""""|_|"""""|_|"""""|_|"""""|_| """ | 
"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-'"`-0-0-' 
Type 'exit' to return to the menu.
```
</details>


## Investigate S3 Bucket

* [Conversation: Shinny Upatree](conversations.md#shinny-upatree)
* [Objective 02](objectives.md#02---investigate-s3-bucket-)

challenge=awsbucket

Usage: https://digi.ninja/projects/bucket_finder.php

Solution:
```bash
cd bucket_finder/; echo "wrapper3000" >> wordlist; ./bucket_finder.rb wordlist --download; cd wrapper3000/
base64 -d package | zcat | bzip2 -d | tar xf - > package.txt.Z.xz.xxd
xxd -r package.txt.Z.xz.xxd | xz -d | gzip -d -
```


## Unescape Tmux
* [Conversation: Pepper Minstix](conversations.md#pepper-minstix)

challenge=tmux

Can you help me?
I was playing with my birdie (she's a Green Cheek!) in something called **tmux**,
then I did something and it disappeared!
Can you help me find her? We were so **attach**ed!!

Solution:
```bash
tmux list-sessions
tmux attach
```


## Javascript Elf Game
* [Conversation: Ribb Bonbowford](conversations.md#ribb-bonbowford)

### Level 1
```javascript
elf.moveTo(lollipop[0])
elf.moveUp(10)
```

### Level 2 - Trigger The Yeeter
```javascript
elf.moveLeft(6)
elf.pull_lever(elf.get_lever(0) + 2)
elf.moveLeft(4)
elf.moveUp(10)
```

## Level 3
```javascript
elf.moveTo(lollipop[0])
elf.moveTo(lollipop[1])
elf.moveTo(lollipop[2])
elf.moveUp(1)
```

## Level 4 - Up Down Loopiness
```javascript
for (var i = 0; i < 3; i++) {
  elf.moveLeft(3)
  elf.moveUp(13)
  elf.moveLeft(3)
  elf.moveDown(13)
}
elf.moveUp(13)
```

## Level 5 - Move To Madness
```javascript
var q = elf.ask_munch(0)
var a = q.filter(elem => typeof elem === 'number')
console.log(q + '\n' + a)
elf.moveTo(lollipop[1])
elf.moveTo(lollipop[0])
elf.tell_munch(a)
elf.moveUp(2)
```

### Level 6 - Two Paths, Your Choice
```javascript
var obj = elf.ask_munch(0)
var a = ""
Object.keys(obj).forEach(function(k) {
  if (obj[k] == 'lollipop') {
    console.log(k + ' - ' + obj[k]);
    a = k;
  }
});
for (var l = 0; l < 4; l++) { elf.moveTo(lollipop[l]) }
elf.moveTo(munchkin[0])
elf.tell_munch(a)
elf.moveUp(2)
```

## Sort-O-Matic
* [Conversation: Minty Candycane](conversations.md#minty-candycane)

challenge=regex

1. Matches at least one digit
```
\d
```
2. Matches 3 alpha a-z characters ignoring case
```
[a-zA-Z]{3}
```
3. Matches 2 chars of lowercase a-z or numbers
```
[a-z0-9]{2}
```
4. Matches any 2 chars not uppercase A-L or 1-5
```
[^A-L1-5]{2}
```
5. Matches three or more digits only
```
^[0-9]{3,}$
```
6. Matches multiple hour:minute:second time formats only
```
^[0-2]?[0-9]{1}:[0-5]{1}[0-9]{1}:[0-5]{1}[0-9]{1}$
```
7. Matches MAC address format only while ignoring case
```
^([0-9a-fA-F]{2}):([0-9a-fA-F]{2}):([0-9a-fA-F]{2}):([0-9a-fA-F]{2}):([0-9a-fA-F]{2}):([0-9a-fA-F]{2})$
```
8. Matches multiple day, month, and year date formats only
```
^(0[1-9]|[12][0-9]|3[01])[- /.](0[1-9]|1[012])[- /.](19|20)\d\d$
```

## Linux Primer
* [Conversation: Sugarplum Mary](conversations.md#sugarplum-mary)

challenge=linux

The North Pole 🍭 Lollipop Maker:
All the lollipops on this system have been stolen by munchkins. Capture munchkins by following instructions here and 🍭's will appear in the green bar below. Run the command "hintme" to receive a hint.

```bash
ls ~
cat munchkin*
rm munchkin*
pwd
ls -la
rm .munchkin*
history
env | grep -i munch
cd workshop/
grep -i munch *
chmod u+x lollipop_engine
./lollipop_engine
cd /home/elf/workshop/electrical
mv blown_fuse0 fuse0
ln -s fuse0 fuse1
cp fuse1 fuse2
echo "MUNCHKIN_REPELLENT" >> fuse2
find /opt/munchkin_den/
find /opt/munchkin_den/
find /opt/munchkin_den/
ps -ef| grep -i munch
netstat -nlpt
curl localhost:54321
kill $(ps -ef | grep -i munchkin | grep -v grep | awk '{print $2}')
exit
```

## Santa Shop
* [Conversation: Sugarplum Mary](conversations.md#sugarplum-mary)
* [Objective 03](objectives.md#03---point-of-sale-password-recovery-)

challenge=

* spin up a nodejs container and extract .asar file from .exe
* find password in main.js

```bash
docker run -it --rm node /bin/bash
apt update && apt install -f wget p7zip p7zip-full less
npm install -g asar
wget https://download.holidayhackchallenge.com/2020/santa-shop/santa-shop.exe
mkdir extracted app source
7z -oextracted/ x santa-shop.exe
7z -oapp/ x extracted/\$PLUGINSDIR/app-64.7z
asar list app/resources/app.asar
asar extract app/resources/app.asar source
rm -rf extracted app
cat README.md
grep PASSWORD main.js
```


## Greeting Cards
* [Conversation: Chimney Scissorsticks](conversations.md##chimney-scissorsticks)

https://greeting-cards.kringlecastle.com/



## Scapy Prepper
* [Conversation: Alabaster Snowball](conversation.md#alabaster-snowball)



## CAN-Bus Investigation
* [Conversation: Wunorse Openslae](conversation.md#wunorse-openslae)

