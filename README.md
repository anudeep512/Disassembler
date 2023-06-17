
# RISC-V Disassembler

This project was done as part of **Course CS2233** which was organized by **Dr. Rajesh Kedia** which aims to develop a Disassembler which converts given **RISC-V machine code** to **RISC-V instruction**


## Authors

- [@anudeep512](https://www.github.com/anudeep512)


## Tech Stack

**Command Line:** C++



## Prerequisite
Check if a suitable compiler exists for compiling the C++ code

for g++ compiler:

    g++ --version
for clang compiler:

    clang --version

Check if CMake exists:

    cmake --version
If there isn't any version of CMake installed on your machine install CMake:

for MacOS:

    brew install cmake 

for Ubuntu:

    sudo apt-get install cmake
## Installation and Usage 

### Installing project

Clone from repo:

    git clone https://github.com/anudeep512/Disassembler/



### Running the Program

After cloning is done redirect control to project folder using:

    cd ./Disassembler

To generate the compilation files run:
    
    cmake .

To actually compile the application, you must use GNU make with the make command:

    make

Launch the application with:

    ./Disassembler




## Features

- Given a **8 digit HEX RISC-V machine code** the corresponding **RISC-V instruction** is generated 

### Example 
#### Input 
    007201b3
    00720863
    00c0006f
    00533623 
    100004b7 
    00c50493

#### Output
    add x3, x4, x7 
    beq x4, x7, L1
    jal x0, L1
    sd x5, 12(x6)
    lui x9, 0x10000
    L1: addi x9, x10, 12

- Sample Test cases can be found in the files **inputs.txt, inputs1.txt, inputs2.txt**. The code reads input from the file **inputs.txt** so work accordingly changing the file.







## Documentation

Please look into https://anudeep512.github.io/RISC-V-Disassembler/ for documentation




