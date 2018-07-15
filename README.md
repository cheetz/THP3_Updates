# THP3_Updates
All Updates for THP3 will be hosted here instead of the website: TheHackerPlaybook.com/updates.  It'll be easier to do it here and readers can also make issue requests.  Thanks! -Peter

THP Book Updates: 

- Some users are having problems unzipping the THP-VM.  If on OSX, try Keka and if on Linux try 7Zip.  For some reason, the native unzip tools don't like the large file.

- Minor typo on the URL for the notes for the Custom Support System VM Web Lab.  Instead of blog it was supposed to be blob.  Updated link: https://github.com/cheetz/THP-ChatSupportSystem/blob/master/lab.txt.  I believe you should be able to update any ebooks copies on Kindle to contain the new link, but of course not physical.  Updated physical for future purchases.
- Knock, minor typo on the command, switch is "-w" and not "-u" (i.e. python ./knockpy.py cyberspacekittens.com -w all.txt)
- Slurp (https://github.com/bbb31/slurp.git) github repo has been removed by the owner.  This tool can still be found on the THP Kali VM under /opt/slurp or on archive.org https://archive.org/details/github.com-bbb31-slurp_-_2017-12-05_23-19-32.
The instructions to build Slurp correctly are (tested in Kali):

  0. apt get install golang 
  1. wget https://archive.org/details/github.com-bbb31-slurp_-_2017-12-05_23-19-32
  2. git clone bbb31-slurp_-_2017-12-05_23-19-32.bundle
  3. mv bbb31-slurp_-_2017-12-05_23-19-32 slurp
  4. mv slurp/vendor slurp/src
  5. export GOPATH=PATH/TO/slurp
  6. go build
  7. ./slurp domain --domain cyberspacekittens.com

- Bit.ly link for the Red Canary Windows ATT&CK Matrix is broken.  The new link is https://github.com/redcanaryco/atomic-red-team/blob/master/atomics/windows-matrix.md.  

- It looks like the latest Windows 10 update might have broken the PowerShell version of Mimikatz.  So the tool like, HideMyPS might not be working properly until they fix this.  More to come on this.


Recommendations from Readers (or from me):

- From @Heliand, a few other tools to help you build out an Active Directory lab/test environment https://github.com/curi0usJack/ADImporter, https://github.com/jaredhaight/PowerShellClassLab, https://github.com/clong/DetectionLab, https://github.com/outflanknl/Invoke-ADLabDeployer

- Red teamers - take your C2 comms to the next level with mod_python - https://labs.nettitude.com/blog/apache-mod_python-for-red-teams/

- From @_P3GLEG, One new vector which you didn't talk about within your book was Docker. Recently, on a lot of engagements I have found docker registry's with no authentication or a simple/stolen password and am able to pull down images. Using https://github.com/P3GLEG/Whaler I have been able to discover credentials, map the open ports to images and use the information to pivot further. It's a great new vector and just wanted to bring it to your attention.
