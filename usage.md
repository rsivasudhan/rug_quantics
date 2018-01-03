#Usage

## Required files:

1. Save the submit\_quantics file in bin directory of Niewupoort cluster.

2. Download the nocl0.inp in your path



## Basic Usage

To use default variables :


_submit\_quantics nocl0.inp_


### To use a specific que

The following command would use an ultrashortq with wall-clock time of 24:00:00 with 1 node and default memory.


_submit\_quantics nocl0.inp ultrashortq_


## Brief usage of the command:

_**submit\_quantics nocl0.inp ultrashortq**_ _-n 2 -m 1200 -t 22:00:00 -u s.rathnachalam -T 1_ 


The above script submits job to ultrashortq , requesting two nodes , 1.2 GB memory,

requested wall-clock time of 22:00:00 (note the maxtime is 24:00:00) , -u flag sends the user an email about job 


-T flag issues the tasks per node (threads)


## Special cases:

It may happen that you are issuing this command from different directory to that of where the _nocl0.inp_ is stored

and you may also want the output in different directory. For those cases append the options with 

 _**submit\_quantics nocl0.inp ultrashortq**_ _-n 2 -m 1200 -t 22:00:00 -u s.rathnachalam -T 1_ -i \path\to\your\nocl0.inp\  -o \path\where\your\output\stored\
