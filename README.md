This repository contains a registration key generator for ST applications. Follow the instructions below to compile the code and generate a registration key.

## Instructions

1. Install GCC (GNU Compiler Collection):

    ```bash
    sudo apt install gcc -y
    ```

2. Download the source code from GitHub:

    ```bash
    wget https://raw.githubusercontent.com/Seehed/applicationSt/main/make-regkey.c -O make-regkey.c
    wget https://raw.githubusercontent.com/Seehed/applicationSt/main/st-common.h -O st-common.h
    ```

3. Compile the code using GCC:

    ```bash
    gcc -o st-keygen make-regkey.c -std=c99 -Wall -Wextra -pedantic -lm
    ```

4. Run st-keygen to generate a registration key (replace `[LicenceHolder]` with the actual name):

    ```bash
    sudo ./st-keygen [LicenceHolder]
    ```

Replace `[LicenceHolder]` with the desired License Holder name (Example EggMeRadio) when running the `st-keygen` command.
