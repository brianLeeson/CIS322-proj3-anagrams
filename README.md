# proj3-anagrams
Vocabularly anagrams game for primary school English language learners
AUTHOR: Brian Leeson, bel@cs.uoregon.edu

## Overview

A simple anagram game designed for English-language learning students in 
elementary and middle school.  
Students are presented with a list of vocabulary words (taken from a text file) 
and an anagram.  The anagram is a jumble of some number of vocabulary words, randomly chosen.  
Students attempt to type vocabularly words that can be created from the  
jumble.  When a matching word is typed, it is added to a list of solved words. 

The vocabulary word list is fixed for one invocation of the server, so multiple
students connected to the same server will see the same vocabulary list but may 
have different anagrams. 

## RUNNING THE APPLICATION
Do NOT enter the virtual enviroment.

Deployment should work "out of the box" with this command sequence:
#sudo apt-get install python3-venv
#git clone <gitURL>
#cd to the cloned repository
#make configure
#make run

The default port is 5000. If your are on your own machine connect at localhost:5000. 
If the server is running on another machine connect at <OtherMachineIP>:5000.
 
TESTING THE APPLICAITON
Test this server by following the RUNNING instructions and attempt to connect to the server.

## To run automated tests, go into the virtual enviroment. 
From inside /proj3-anagrams:
. /env/bin/activate
nosetests

To exit:
deactivate

There are currently nose tests for vocab.py, letterbag.py, and jumble.py. 
