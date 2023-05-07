# MMGBSA Calculation from Schrodinger thermal_mmgbsa.py

## Run the script

Go to the folder that have the out.cms trajectory file. You can check the existing files by ls

Then run the script-

where:-
xx-out.cms=simulaiton out file
Y=GPU
YY=The simulation frames gap
Z=Number of prime subjobs to create (Make sure Z>Y, or Z=Y)

```bash
$SCHRODINGER/run thermal_mmgbsa.py xx-out.cms -HOST 'localhost:Y' -step_size YY -NJOBS Z
```

## Set Schrodinger Environment variable path

If the command `$SCHRODINGER/run` shows that the `/run is a directory` it means that the the SCHRODINGER environment variable path is not set. To set the environment variable path follow the below code:

```bash
export SCHRODINGER=installdir
```

The `installdir` is where the schrodinger is installed, mostly in `/opt/schrodinger-version`

[Read more](http://gohom.win/ManualHom/Schrodinger/Schrodinger_2015-2_docs/general/unix_quick_install.pdf?fbclid=IwAR0ARRwtmfJxrwG_1b2R7BlwDxbFXjpZ95FM-gcXDsSVCCc_Vn1TDPQXNXM)
