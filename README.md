# How to get deepmd and or lammps to work if you have a MAC
This document is designed for people who have access to HPC at the University of Southern California.

I decided to install deepmd and/or lammps on hpc because it didn’t work for me at all on my local computer.

### Step 1: log onto HPC, install Anaconda (if not already installed) and create a work directory.

### Step 2: install deepmd & lammps

`conda create -n deepmd deepmd-kit=*=*cpu libdeepmd=*=*cpu lammps-dp -c https://conda.deepmodeling.org`

### Step 3: activate deepmd

`conda activate deepmd`

### Step 4: CHECK if things are installed correctly!

`dp -h`
`lmp -h`

### Step 5: run lammps

Upload files such as the .in, .input, .pb to a folder, then start the run use
`lmp < [input file name]`
e.g. `lmp < input.in`
