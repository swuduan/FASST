# FASST-Z3Score - One Click Automatic Sleep Scoring

FASST-Z3Score is a fork of FASST toolbox (fMRI Artefact rejection and Sleep Scoring Toolbox, see below). It includes modifications to allow automatic scoring using the z3score.com sleep scoring API. Read about the API here: https://github.com/amiyapatanaik/z3score-api 
The API uses a three step process (which is transparent to the user):
1. Convert data to compressed feature set (CFS) format. One night sleep record takes approximately 10MBs irrespective of how big the original EDF file is. 
2. Upload data to z3score server
3. receive sleep scores and confidence

To be able to score using z3score API, you will need a license key. Request a key from testdrive@z3score.com 

## Dependencies
**SPM-12**: You will need SPM-12 to use the toolbox. Download SPM 12 from http://www.fil.ion.ucl.ac.uk/spm/software/spm12/ 
**cfslib-MATLAB**: CFS MATLAB library to convert raw data to compressed feature set. Already included here.

# See it in action
[![FASST-Z3Score Demo](https://img.youtube.com/vi/kTPDIZSy15E/maxresdefault.jpg)](https://www.youtube.com/watch?v=kTPDIZSy15E)

For more information visit z3score.com 

(c)-Amiya Patanaik, 2017, Patents pending

This software is released under GPL. 

# FASST

FASST, aka. fMRI Artefact rejection and Sleep Scoring Toolbox, public distribution with the latest updates.
For more info about FASST, see http://www.montefiore.ulg.ac.be/~phillips/FASST.html

A reference paper is available here:
http://hdl.handle.net/2268/89380

This Git/SVN open repository allows us to distribute FASST public version more regularly with bug fixes and the latest features. And end-users can directly update their version by synchronizing with this repository.
A Wiki is also available (though empty at the moment) and problems/bugs can be officially notified through the "Issues" interface.

#### Notes:
* On *March 2, 2016*, FASST is at last compatible with SPM12!
Appologies for the delay, code was used internally but never updated on the public repository...
* The artefact detection tool, published in here http://www.sciencedirect.com/science/article/pii/S0165027015003994, is NOT ready yet to be used by the public. We are working on the remaining issues and hope to make the code available ASAP.
