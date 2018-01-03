# rug\_quantics
This repository  hosts the information related to Quantics (A Quantum dynamics package)
## Scripts
This repository also hosts various scripts that can be used for the theoretical and computational chemistry research. All the scripts provided here are self-explanatory. Any issues regarding the code can be reported to [sivasudhan](mailto:s.rathnachalam@rug.nl)
### submit\_quantics
This script submits the quantics job in the Nieuwpoort cluster of RUG.


**It is highly recommended that you save the _submit\_quantics_ in your bin folder of the account as submit\_quantics**. Learn more about bin folder [here](https://askubuntu.com/questions/406491/how-to-create-and-link-a-bin-folder-to-contain-executables)


### Usage of the script
Usage of the script is explained and it can be obtained 

_ To submit the file with default que variables: _

**_submit\_quantics_** **file.inp** 


**_Wondering what the default Que variables are? _**
Type submit\_quantics default


**_ Want to choose a different Que ? _**
Type _submit\_quantics qinfo_ 

You can also use the script with default variables of different ques available. This choice provides the user with the maximum wall-clock time allowed, memory, tasks per node etc for the particular que chosen!

To exploit this one should use :
_submit\_quantics file.inp qname_

To override the default variables of the que, one may use the optional variable which should be followed by the input file and qname . 

_submit\_quantics file.inp qname **options**_

The order of the arguments for input file and qname is important i.e, file.inp is always the first argument and qname is always the second argument. However, the following optional arguments can be given in any order.

###Optional arguments are :
-n for nodes
-m for requesting memory
-t for time (in hh:min:sec)
-u for recieving job related email (give just the username of your rug mail)
-s on setting this flag to **0** , the script file will  be generated without submitting it!
-T sets tasks per node
-i sets explicit input dir
-o sets explicit output dir

