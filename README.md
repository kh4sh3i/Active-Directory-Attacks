# ActiveDirectory
A curated list of awesome ActiveDirectory Pentesting resources

## [Bloodhound](https://github.com/BloodHoundAD/BloodHound)
is an amazing tool which can enumerate a domain automatically, save all the information, find possible privilege escalation paths and show all the information using graphs.

### install 
* linux 
```
apt-get install bloodhound
```

* windows
  * [Install Java](https://www.oracle.com/java/technologies/javase-jdk11-downloads.html)
  * [Install neo4j](https://neo4j.com/download-center/#community)
  * [Download the BloodHound GUI](https://github.com/BloodHoundAD/BloodHound/releases)

Tips:
```
you should download BloodHound-win32-x64.zip
after execute neo4j you should reset password and after click on BloodHound.exe you should use this credential
by default BloodHound does not any data and you should use SHarpHound for gather information
```

### DATA COLLECTION (ingestor)
* [SharpHound](https://github.com/BloodHoundAD/BloodHound/tree/master/Collectors) SharpHound is the official data collector for BloodHound. It is written in C# and uses native Windows API functions and LDAP namespace functions to collect data from domain controllers and domain-joined Windows systems. 
```
C:\> SharpHound.exe
```

* [BloodHound.py](https://github.com/fox-it/BloodHound.py) If you have domain credentials you can run a python bloodhound ingestor from any platform so you don't need to depend on Windows.

```
pip3 install bloodhound
bloodhound-python -u support -p 'yourpassword' -ns 10.10.10.192 -d blackfield.local -c all
```






### Refrences
https://github.com/chryzsh/awesome-bloodhound

