# CSV files

There are three CSV files necessary for functional logic:
    - conditions_hardware;
    - conditions_existing_software;
    - conditions_planning_software.

## Hardware implementation conditions

For an hardware implementation of security algorithms the variables that have an impact are:
    - Security requirement (Confidentiality, Privacy, among others);
    - Usage of stream cipher (1, 0 or none);
    - Is it a sensitive domain (1 or 0);
    - Max dimension for circuit area;
    - Min dimension for circuit area;
    - Max throughput;
    - Min throughput;
    - Hardware type (ASIC or FPGA, until now);
    - Energy performance (Low or Super Low, until now);
    - Recommendation ID (Found in the database).

The recommendation should be given when all the conditions are fulfilled by the user's system.
If the security requirement doesn't use ciphers then there is no need to refer to the stream cipher condition. The correspondant column should be empty, as in the example below:
`Integrity, ,1,...`

Also, if the logic file needs to compare strings don't leave any space between commas.

## Software implementation conditions

The need to implement a software implementation of security algorithms can happen in two ways, either the system already **exists** or it is being **planned**.

### Existing system

If the system already exists the relevant variables are:
    - Security requirement (Confidentiality, Privacy, among others);
    - Usage of stream cipher (1, 0 or none);
    - Is it a sensitive domain (1 or 0);
    - Max size for flash memory;
    - Min size for flash memory;
    - Max size for RAM;
    - Min size for RAM;
    - Hardware type (AVR, MSP, ARM, until now);
    - Recommendation ID (Found in the database).

### Planning system

If the system is being planned the relevant variables are:
    - Security requirement (Confidentiality, Privacy, among others);
    - Usage of stream cipher (1, 0 or none);
    - Is it a sensitive domain (1 or 0);
    - Max size for flash memory;
    - Min size for flash memory;
    - Max size for RAM;
    - Min size for RAM;
    - CPU bits (8, 16, 32, 64, until now);
    - Recommendation ID (Found in the database).

The recommendation should be given when all the conditions are fulfilled by the user's system.
If the security requirement doesn't use ciphers then there is no need to refer to the stream cipher condition. The correspondant column should be empty, as in the example below:
`Integrity, ,1,...`

Also, if the logic file needs to compare strings don't leave any space between commas.
