## Kringle Kiosk
* Location: Castle Approach
* [Conversation: Shinny Upatree](conversations.md#shinny-upatree)

<details><summary>Click to expand</summary>

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
* Location: Castle Approach
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
* Location: Castle Approach
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


## The Elf Code
* Location: Dining Room
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
* Location: Workshop
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
* Location: Courtyard
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
* Location: Courtyard
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

## 33.6kbps
* Location: Kitchen
* [Conversation: Fitzy Shortstack](conversations.md#fitzy-shortstack)

```
Pick up handset
Dial 'SKOUDIS' (756-8347)
Click 'baa DEE brrr'
Click 'aaah'
Click 'WEWEWWRWRRWRR'
Click 'beDURRdunditty'
Click 'SCHHRRHHRTHRTR'
```

## HID Lock
* Location: Workshop
* [Objective 05](objectives.md#05---open-hid-lock-)

* Use your Proxmark3 in your Badge Items inventory to scan Shinny Upatree's HID badge

```
[magicdust] pm3 --> lf hid read
#db# TAG ID: 2006e22f13 (6025) - Format Len: 26 bit - FC: 113 - Card: 6025
[+] Valid HID Prox ID found!
```

* Simulate that card in front of the locked door in the Workshop

```
[magicdust] pm3 --> lf hid sim -r 2006e22f13 --fc 113 --cn 6025
[=] Simulating HID tag using raw 2006e22f13
[=] Stopping simulation after 10 seconds.
[=] Done
```

* Location: ???

Become Santa?!?


## Speaker UNPrep
* Location: Talks Lobby
* [Conversation: Bushy Evergreen](conversations.md#bushy-evergreen)

challenge=santamode-speaker

### Open the door

Super simple

```bash
strings door|grep -i password
```

**Answer**: Op3nTheD00r


### Turn on the lights

Here are a few commands that can be run to dump the memory heap of the process to a file, where you can see the decrypted password in plain text.

```bash
# start term
./lights
# ctrl + z

cd lab;
pid=$(jobs -p)
addrs=$(grep rw-p /proc/${pid}/maps | grep heap | awk '{print $1}')
start=$(echo $addrs | cut -d- -f1)
stop=$(echo $addrs | cut -d- -f2)
gdb --batch --pid ${pid} -ex "dump memory pid${pid}-heap-$start-$stop.dump 0x$start 0x$stop"
strings pid*heap*.dump

# there's the password, now go enter it!
/home/elf/lights
```

**Answer**: Computer-TurnLightsOn

### Turn on the vending machine

I wrote a short bash script to cycle through input characters and see how the encoded output changes. 

```bash
echo "Match this: LVEdQPpBwr"
known="$1"
for i in {a..z} {A..Z} {0-9}; do
  rm vending-machines.json;
  echo -e "me\n${known}${i}" | ./vending-machines >/dev/null
  out=$(cat vending-machines.json | grep password | awk -F: '{print $2}')
  echo "${known}${i} ->$out"
done
```

To start, you just run the script, and it automates the process of deleting the json file, running the binary, giving it an input, and reading the resulting output from the new json. Once you find a match for the first character, you stop the script and re-run it with the inputs you already know, and continue until you have every character of the password. I could automate this further, to grep for a match so it runs completely on its own, but this worked fine as is.

**Answer**: CandyCane1


## Splunk
* Location: Great Room
* [Conversation: Angel Candysalt](conversations.md#angel-candysalt)
* [Objective 06](objectives.md#06---splunk-challenge-)

https://splunk.kringlecastle.com/en-US/app/SA-kringleconsoc/kringleconsoc

### Training Questions

1.	How many distinct MITRE ATT&CK techniques did Alice emulate?

Splunk Query:
```
| tstats count where index=t* by index 
| rex field=index mode=sed "s/(\.|-).*$//" 
| dedup index
```

```
= 13
```


2.	What are the names of the two indexes that contain the results of emulating Enterprise ATT&CK technique 1059.003? (Put them in alphabetical order and separate them with a space)

```
= t1059.003-main t1059.003-win
```


3.	One technique that Santa had us simulate deals with 'system information discovery'. What is the full name of the registry key that is queried to determine the MachineGuid?

https://attack.mitre.org/techniques/enterprise/

search for "system information discovery"

https://attack.mitre.org/techniques/T1082/


Splunk Query:
```
| tstats count where index=* by index 
| rex field=index "(?<technique>t\d+)[\.\-].0*"
|  search technique=t1082
```

Splunk Query:
```
index=t1082-win MachineGuid
```

```
= HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Cryptography
```


4.	According to events recorded by the Splunk Attack Range, when was the first OSTAP related atomic test executed? (Please provide the alphanumeric UTC timestamp.)

Splunk Query:
```
index=attack OSTAP 
| stats values(Execution Time _UTC) by _time
```

```
= 2020-11-30T17:44:15Z
```


5.	One Atomic Red Team test executed by the Attack Range makes use of an open source package authored by frgnca on GitHub. According to Sysmon (Event Code 1) events in Splunk, what was the ProcessId associated with the first use of this component?

https://github.com/frgnca/AudioDeviceCmdlets

Splunk Query:
```
index=attack audio
```

Splunk Query:
```
| tstats count where index=* by index 
| rex field=index "(?<technique>t\d+)[\.\-].0*"
|  search technique=t1123
```

Splunk Query:
```
index=t1123-win EventID=1 ProcessId ParentCommandLine="*powershell.exe*"
| dedup ParentCommandLine
| stats values(ParentCommandLine) by ProcessId, _time
| sort _time
```

```
= 3648
```


6.	Alice ran a simulation of an attacker abusing Windows registry run keys. This technique leveraged a multi-line batch file that was also used by a few other techniques. What is the final command of this multi-line batch file used as part of this simulation?

Splunk Query:
```
index=attack registry
```

Splunk Query:
```
| tstats count where index=* by index 
| rex field=index "(?<technique>t\d+)[\.\-].0*"
|  search technique=t1547
```

Splunk Query:
```
index=t1547.001-win EventID=1 ProcessId ParentCommandLine="*powershell.exe*"
| dedup ParentCommandLine
| stats values(ParentCommandLine) by ProcessId, _time
| sort _time
```


https://attack.mitre.org/techniques/T1547/001/

Splunk Query:
```
index=* file_name="*.bat" 
| stats values(file_name)
```

Discovery.bat

https://github.com/redcanaryco/atomic-red-team/blob/master/ARTifacts/Misc/Discovery.bat

```
= quser
```


7.	According to x509 certificate events captured by Zeek (formerly Bro), what is the serial number of the TLS certificate assigned to the Windows domain controller in the attack range?

Splunk Query:
```
index=* sourcetype=bro* source="/opt/zeek/logs/current/x509.log" "certificate.issuer"="CN=win-dc*"
| stats values(certificate.serial) by certificate.issuer
```

```
= 55FCEEBB21270D9249E86F4B9DC7AA60
```


8. Challenge Question: What is the name of the adversary group that Santa feared would attack KringleCon?

RFC 7465 = Prohibiting RC4 Cipher Suites

https://gchq.github.io/CyberChef/#recipe=From_Base64('A-Za-z0-9%2B/%3D',true)RC4(%7B'option':'UTF8','string':'Stay%20Frosty'%7D,'Latin1','Latin1')&input=N0ZYalAxbHlmS2J5REsvTUNoeWYzNmg3

```
= The Lollipop Guild
```


## CAN-Bus Investigation
* Location: Roof / NetWars
* [Conversation: Wunorse Openslae](conversations.md#wunorse-openslae)
* [Conversation: Wunorse Openslae to Santa](conversations.md#wunorse-openslae-to-santa)

challenge=santamode-canbus

```bash
$ cat candump.log | awk '{print $3}' | sort | uniq -c | head
     35 188#00000000
      2 19B#000000000000   ## Lock?
      1 19B#00000F000000   ## Unlock?
      1 244#0000000012
      1 244#0000000024
      1 244#0000000036
      1 244#0000000048
      1 244#000000005A
      1 244#000000006C
      1 244#000000007E

$ cat candump.log | grep 19B                                
(1608926661.626380) vcan0 244#000000019B
(1608926662.390980) vcan0 244#000000019B
(1608926664.626448) vcan0 19B#000000000000  ## Lock?
(1608926667.837300) vcan0 244#00000019BE
(1608926671.122520) vcan0 19B#00000F000000  ## Unlock?
(1608926673.157900) vcan0 244#00000019BE
(1608926674.092148) vcan0 19B#000000000000  ## Lock?

$ grep "19B#00000F000000" candump.log
(1608926671.122520) vcan0 19B#00000F000000

$ ./runtoanswer 122520
Your answer: 122520
Checking....
Your answer is correct!
```


## Sleigh CAN-D-Bus
* Location: Roof / NetWars
* Conversation: Wunorse Openslae

challenge=candbus




## Greeting Cards
* Location: Talks Lobby
* [Conversation: Chimney Scissorsticks](conversations.md#chimney-scissorsticks)

https://greeting-cards.kringlecastle.com/



## Scapy Prepper
* Location: Roof / NetWars
* [Conversation: Alabaster Snowball](conversations.mds#alabaster-snowball)






## Tag Generator
* Location: Wrapping Room
* [Conversation: Noel Boetie](conversations.md#noel-boetie)
* [Conversation: Noel Boetie to Santa](conversations.md#noel-boetie-to-santa)
* [Conversation: Holly Evergreen to Santa](conversations.md#holly-evergreen-to-santa)
* [Conversation: Shinny Upatree to Santa](conversations.md#shinny-upatree-to-santa)

https://tag-generator.kringlecastle.com/


## Snowball Fight
* Location: Speaker UNPreparedness Room
* Conversation: Tangle Coalbox

challenge=santamode-snowball


## Naughty/Nice List
* Location: Santa's Office

https://download.holidayhackchallenge.com/2020/blockchain.dat


## ARP Shenanigans
* Location: Roof / NetWars
* Conversation: Alabaster Snowball

challenge=santamode-arp



