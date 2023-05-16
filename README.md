# stellar_structure_final_project
Calculation of the Zero-Age Main Sequence Structure of the Sun

The Jupyter notebook final_project.ipynb should run up until Part 11 (which uses MESA). Below are instructions on how to run the MESA component of this notebook. 

Step 1: Run `git clone https://github.com/myunus1/stellar_structure_final_project.git`

Step 2: Download the MESA zip file using the installation instructions at `https://docs.mesastar.org/en/release-r22.11.1/installation.html` 

Step 3: Move the directory `mesa-r22.11.1/` into `stellar_structure_final_project/'

Step 4: In `~/.bash_profile`, change the line `export MESA_DIR=/Users/jschwab/Software/mesa-r21.12.1` to reflect the new location of `mesa-r22.11.1/`

Step 5: Compile MESA according to the installation instructions

Step 6: Follow the tutorial on using MESA at `https://docs.mesastar.org/en/release-r22.11.1/using_mesa/running.html` but use the following lines instead of the ones given: 

```
$ cp -r $MESA_DIR/star/work sun
$ cd sun
$ ./mk
```

Step 7: In the `sun/` directory, replace the files `inlist`, `inlist_project`, and `inlist_pgstar` with the ones given in this repository

Step 8: Execute `./rn` - should be good to go!
