![wiki](https://github.com/charanravi-online/wiki/blob/main/snap_icon/wiki_banner.png)



[![wiki](https://snapcraft.io/wiki/badge.svg)](https://snapcraft.io/wiki)
[![wiki](https://snapcraft.io/wiki/trending.svg?name=0)](https://snapcraft.io/wiki)



# About this repo
1. This repository utilises the python application from the https://github.com/charanravi-online/terminal-wiki and adds configuration that packages the python app into a snap application using snapcraft.yaml file. 

# How to install?
## Linux

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/wiki)

## Windows

Download and install the latest ```install_wiki.exe``` from the [release page](https://github.com/charanravi-online/wiki/releases/tag/v1.0)


**Note:** Since this is an unsigned exe file, Windows could flag it as a potential threat and prompt you to click on ```Don't Run```.\
There are two ways to tackle this.

1. You can ignore the promp and click on ```More info``` and it should show another button ```Run Anyway``` right next to ```Don't Run```.\
   Click on ```Run anyway``` and the application should install normally.
3. Right click the file and select ```Properties```.\
   Under the ```General``` tab, near the bottom, you'll see ```This file came from another computer and might be blocked to help protect this computer```.\
   Select ```Unblock``` and click ```Apply``` or ```OK```.\
   Now you should be able to double click on the installer and install the application noramlly.

<details>
<summary><h3>Why is the windows installer not signed?</h3></summary>
It costs quite a lot to get an application signed (and I cannot afford it), hence the workarounds mentioned above.
If you're interested in this project and want to sponsor a certificate,
you can do so by reaching out to me via mail: charanravi-online@gmail.com
</details>

## Mac
Coming Soon 👀






<!---## Other ways to install on Windows (OLD METHOD, NOT RECOMMENDED)
Since it is a python appication in its core, it can be installed using the setup.py file.\
**Prerequisites:** Python & pip must be installed oin your machine.
1. Clone the repo
2. Navigate to the path where ```setup.py``` is present.
3. Run ```python setup.py install```
4. Now you should be able to use wiki.
5. To uninstall just run ```pip uninstall wiki```-->




# Build your own windows installer using the source code

1. Once you've cloned this repo, running ```pyinstaller.exe --onefile .\src\wiki.py``` will generate two folders ```build/``` & ```dist/```.The ```wiki.exe``` will be located in ```dist/```
2. LICENSE.txt, POST_INSTALL_INFO.txt & PRE_INSTAL_INFO.txt are useful information files required to package the wiki.exe file.
3. The win_installer folder contains install_wiki.iss (make sure to change the file paths accordingly) script that can be run by the [inno setup compiler](https://jrsoftware.org/isdl.php).\
Simply run the script using inno setup compiler and you should generate a Output folder inside win_installer folder. This folder will contain ```install_wiki.exe``` which is our final installation file.


~~Note: Bare in mind that it may not perform as expected on a Windows machine, since it was build for/on Linux machines.
Please do report bugs if you find any, I'll try my best to optimise it for all the platforms as I can.~~


# How to use?

```wiki "your search query here"```


You will be presented with a list of items your search query matches with. Pick one of them and a short summary will be displayed.\
Then summary related to the page you select will be displayed.



# Example

Here's an example of how to use the script:

```
charan@charan ~> wiki "the conjuring"
Here are the results for: "the conjuring"
1. The Conjuring - The Conjuring is a 2013 American supernatural horror film directed by James Wan and written by Chad Hayes and Carey W. Hayes. It is the inaugural film...

2. The Conjuring Universe - The Conjuring Universe is an American horror franchise and shared universe centered on a series of supernatural horror films. The franchise is produced...

3. The Conjuring 2 - The Conjuring 2 (known in the United Kingdom as The Conjuring 2: The Enfield Case) is a 2016 American supernatural horror film, directed by James Wan....

4. The Conjuring: The Devil Made Me Do It - James Wan. The film serves as a sequel to The Conjuring (2013) and The Conjuring 2 (2016), and as the seventh installment in The Conjuring Universe. Patrick...

5. Conjuration - Look up conjuration or conjuring in Wiktionary, the free dictionary. Conjuration or Conjuring may refer to: Conjuration (summoning), the evocation of spirits...

6. Conjuring Kannappan - Conjuring Kannappan (also marketed as Conjuring Kannappan: Dreams Come True) is a 2023 Indian Tamil-language comedy horror film written and directed by...

7. Ed and Lorraine Warren - This story serves as the inspiration for The Conjuring: The Devil Made Me Do It (2021). The case was described in the 1983 book The Devil in Connecticut...

8. The Conjuring (soundtrack) - The Conjuring (Original Motion Picture Soundtrack) is the score album to the 2013 film The Conjuring directed by James Wan. The film score is composed...

9. The Nun (2018 film) - serves as a spiritual spin-off to The Conjuring 2 and is the fifth installment in The Conjuring shared universe. The film stars Taissa Farmiga, Demián...

10. The Conjuring (song) - "The Conjuring" is a song by the thrash metal band Megadeth from their 1986 album Peace Sells... but Who's Buying?. Written by Dave Mustaine during a...

Pick a page: 1
Directed by: James Wan
Written by: Chad Hayes
Carey W. Hayes
Produced by: Tony DeRosa-Grund
Peter Safran
Rob Cowan
Starring: Vera Farmiga
Patrick Wilson
Ron Livingston
Lili Taylor
Cinematography: John R. Leonetti
Edited by: Kirk Morri
Music by: Joseph Bishara
Productioncompanies: New Line Cinema
The Safran Company
Evergreen Media Group
Distributed by: Warner Bros. Pictures
Release dates: July 15, 2013 (2013-07-15) (Cinerama Dome)
July 19, 2013 (2013-07-19) (United States)
Running time: 112 minutes
Country: United States
Language: English
Budget: $20 million
Box office: $319.5 million
Summary:
The Conjuring is a 2013 American supernatural horror film directed by James Wan and written by Chad Hayes and Carey W. Hayes. It is the inaugural film in The Conjuring Universe franchise. Patrick Wilson and Vera Farmiga star as Ed and Lorraine Warren, paranormal investigators and authors associated with prominent cases of haunting. Their purportedly real-life reports inspired The Amityville Horror story and film franchise. The Warrens come to the assistance of the Perron family, who experienced increasingly disturbing events in their newly occupied farmhouse in Rhode Island in 1971.
Read more: https://en.wikipedia.org/wiki/The_Conjuring
charan@charan ~> 

```

The script will then fetch and parse the information from the page on Wikipedia and print it to the terminal.

# contribution guidelines
Refer the [CONTRIBUTION](https://github.com/charanravi-online/wiki/blob/main/docs/CONTRIBUTING.md) for contribution guidelines before making any contributions.

