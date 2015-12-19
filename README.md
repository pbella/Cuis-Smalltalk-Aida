Aida
====

AidaWeb Smalltalk Web Application Server for Cuis 4.2

Port of Aida Web (http://www.aidaweb.si) to Cuis Smalltalk 4.2

Taken from Aida6.5-interim.2 from the repo http://www.smalltalkhub.com/#!/~Aida/Aida/versions/Aida6.5-interim.2

Updated to work with Cuis 4.2 2595

You will need to download the following git repositories as well:
https://github.com/pbella/Cuis-Smalltalk-Cryptography
https://github.com/pbella/Cuis-Smalltalk-Pharo14CompatibilityLayer
https://github.com/pbella/Cuis-Smalltalk-CompatibilityWithOtherSmalltalks
https://github.com/pbella/Cuis-Smalltalk-Sport
https://github.com/pbella/Cuis-Smalltalk-Swazoo

If you then copy all of the packages (*.pck.st) from the above repos as well as the Aida package from this repository into your local Cuis package directory, you can install by executing:
````Smalltalk
	Feature require: 'Network-Kernel'.
Smalltalk
	Feature require: 'Aida'.
AIDASite initialize
````

Notes:
- Disabled hourly snapshots in AIDASite>>initHourlySnapshot
- AIDA demo does not start by default, hence the need to call 'AIDASite initialize'

Thanks to Germán Arduino for his work originally porting all of this!
