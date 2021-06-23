# Random and Pseudorandom Number Generators for Cryptographic Applications 


## Statistical Test Suite for Random and Pseudorandom Number Generators for Cryptographic Applications (NIST)

This toolbox was created especially for those involved in statistical testing of cryptographic (P)RNGs. The problem of evaluating (P)RNGs for randomness will be addressed by this bundle. 
It will be useful for: 

* identifying (P)RNGs that generate poor (or patterned) binary sequences, 
* designing new (P)RNGs, 
* verifying that (P)RNG implementations are right, 
* studying (P)RNGs defined in standards, 
* investigating the degree of randomness generated by currently used (P)RNGs.


It can be downloaded on https://csrc.nist.gov/projects/random-bit-generation/documentation-and-software. The instructions for the use of this tool can be found in the link above in chapter 5.

To set up the tool the user needs to:

* Copy the sts.tar file into the root directory. Use the instruction, tar -xvf sts.tar, to unbundle the source code. 
* Six subdirectories and one file should have been created.  The subdirectories are: data/, experiments/, include/, obj/, src/ and templates/. The file is makefile. 
* Edit the makefile.  Modify the following lines: (a) CC (your ANSI C compiler) (b) ROOTDIR (the root directory that was prescribed earlier in the process, e.g., rng/) 
* Now execute makefile.  An executable file named assess should appear in the project directory. 
* The data may now be evaluated.  Type the following: 

``` bash
    assess <sequenceLength>
```