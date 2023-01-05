This repository contains the source codes for the paper, 'Restricted Near Collision Attack on Plantlet'.

## Software Used
1. [Sagemath](https://www.sagemath.org/)
2. [Cryptominisat](https://github.com/msoos/cryptominisat)


## Setup

1. To install sagemath in conda environment:
	a. 'conda config --add channels conda-forge'
	b. 'conda config --set channel_priority strict'
	c. 'conda create -n sage sage python=3.8'

2. Activate the new environment: 'conda activate sage'
3. Install the required package cryptominisat : `conda install -c conda-forge cryptominisat` and 'conda install -c conda-forge libcryptominisat'



## File Structure

1. `1_Plantlet_fixed_0-1_type1_equ_type2_equ.sage`: Script for finding the position of fixed 0/1 in the xor difference keystream for some fixed difference in the LFSR of the internal state. Also find the type1 and type2 equations and their positions.

2. `2_Plantlet_Encryption.sage`: Script to measure the average encryption time for 1 Plantlet encryption

3. `3_Plantlet_UNSAT_time.sage`: Script to mesure the average UNSAT time for solving system of nonlinear equations.

3. `4_Plantlet_SAT_time.sage`: Script to mesure the average SAT time for solving system of nonlinear equations.



## Usage
step 1: activate sagemath by running the command 'conda activate sage'
step 2: compile and run by the command 'sage file_name.sage' 

note: for running first programme run the command 'sage 1_Plantlet_fixed_0-1_type1_equ_type2_equ.sage'
