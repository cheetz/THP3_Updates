# THP3_Updates
All Updates for THP3 will be hosted here instead of the website: TheHackerPlaybook.com/updates.  It'll be easier to do it here and readers can also make issue requests.  Thanks! -Peter

THP Book Updates: 

- Minor typo on the URL for the notes for the Custom Support System VM Web Lab.  Instead of blog it was supposed to be blob.  Updated link: https://github.com/cheetz/THP-ChatSupportSystem/blob/master/lab.txt.  I believe you should be able to update any ebooks copies on Kindle to contain the new link, but of course not physical.  Updated physical for future purchases.

- Slurp was not working as intended in the THP Virtual Kali Machine.  All images on the server have been updated, but if you want to manually update it, you can do this:
  - git clone https://github.com/bbb31/slurp.git /opt/slurp && cd /opt/slurp && cp /root/go/bin/slurp /opt/slurp/
  - ./slurp domain -t cyberspacekittens.com




Recommendations from Readers (or from me):

- From @Heliand, a few other tools to help you build out an Active Directory lab/test environment https://github.com/curi0usJack/ADImporter, https://github.com/jaredhaight/PowerShellClassLab, https://github.com/clong/DetectionLab, https://github.com/outflanknl/Invoke-ADLabDeployer

- Red teamers - take your C2 comms to the next level with mod_python - https://labs.nettitude.com/blog/apache-mod_python-for-red-teams/
