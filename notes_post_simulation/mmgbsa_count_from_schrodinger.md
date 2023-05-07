# MMGBSA Calculation from Schrodinger thermal_mmgbsa.py

## Run the script

Go to the folder that have the `out.cms` trajectory file. You can check the existing files by ls

Then run the script-

where:- </br>
xx-out.cms=simulaiton out file </br>
Y=GPU </br>
YY=The simulation frames gap </br>
Z=Number of prime subjobs to create (Make sure Z>Y, or Z=Y)

```bash
$SCHRODINGER/run thermal_mmgbsa.py xx-out.cms -HOST 'localhost:Y' -step_size YY -NJOBS Z
```

Example:

```bash
$SCHRODINGER/run thermal_mmgbsa.py desmond_md_job_2-out.cms -HOST 'localhost:4' -step_size 20
```

![image](images/mmgbsa.png "MMGBSA Script")

It will generate a .csv result output file.

## Setup: Set Schrodinger Environment variable path

If the command `$SCHRODINGER/run` shows that the `/run is a directory` it means that the the SCHRODINGER environment variable path is not set. To set the environment variable path follow the below code:

```bash
export SCHRODINGER=installdir
```

The `installdir` is where the schrodinger is installed, mostly in `/opt/schrodinger2023-1`

[Read more](http://gohom.win/ManualHom/Schrodinger/Schrodinger_2015-2_docs/general/unix_quick_install.pdf?fbclid=IwAR0ARRwtmfJxrwG_1b2R7BlwDxbFXjpZ95FM-gcXDsSVCCc_Vn1TDPQXNXM)

Sometimes after restart the terminal the environment variable may lost, so to add the schrodinger environment permanently follow the steps:

1. open bashrc by `sudo nano .bashrc`
2. Then add the code at the bottom `export SCHRODINGER="/opt/schrodinger2023-1"`
3. Reload the bashrc by `source ~/.bashrc`
4. Now check the path was added or not by `echo $SCHRODINGER`, If the code returns `/opt/schrodinger2023-1` that means the path added permanently.
5. Now you may run `$SCHRODINGER/run` from anywhere of you machine
