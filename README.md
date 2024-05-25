# RSA Matrix Encryption

This project demonstrates a simple RSA matrix encryption system using Python and a Makefile to automate the process. The system reads a text input, converts it to numerical values, and performs encryption using a matrix transformation.

## Files

- **Makefile**: Contains instructions for compiling and running the program.
- **rsa_matrix.py**: The main Python script that performs the encryption.
- **test.txt**: A sample text file used as input for the encryption process.

## Requirements

- Python 3.x
- NumPy

## Setup

1. Ensure you have Python 3.x installed on your system.
2. Install NumPy by running:
   ```bash
   pip install numpy
   ```

## Usage

To run the encryption process with the provided sample input:

1. Open a terminal.
2. Navigate to the project directory.
3. Run the following command:
   ```bash
   make run < test.txt
   ```

## Example Output

When running the command `make run < test.txt`, the output should look similar to this:

```
What is a word that you want to safely transmit?(MAX 33 characters):
LOREM IPSUM IS SIMPLY DUMMY TEXT
[11, 14, 17, 4, 12, -33, 8, 15, 18, 20, 12, -33, 8, 18, -33, 18, 8, 12, 15, 11, 24, -33, 3, 20, 12, 12, 24, -33, 19, 4, 23, 19]
[11, 14, 17, 4, 12, -33, 8, 15, 18, 20, 12, -33, 8, 18, -33, 18, 8, 12, 15, 11, 24, -33, 3, 20, 12, 12, 24, -33, 19, 4, 23, 19]
[[ 0  1]
 [ 0 26]
 [ 1 26]
 [ 0 26]]
[[ 11  12  18   8   8  24  12  19]
 [ 14 -33  20  18  12 -33  12   4]
 [ 17   8  12 -33  15   3  24  23]
 [  4  15 -33  18  11  20 -33  19]]
[[ 1  5  9]
 [ 2  6 10]
 [ 3  7 11]
 [ 4  8 12]]
ABAAAABABBBBBBBA
6AD28D)
        -$;CG08P$$$9K^O8
LOREM IPSUM IS SIMPLY DUMMY TEXT
```

## Explanation

1. **Input**: The user is prompted to input a word or phrase (maximum 33 characters).
2. **Numerical Conversion**: The input text is converted into a list of numerical values corresponding to the characters.
3. **Matrix Encryption**: The numerical values are transformed using a predefined matrix.
4. **Output**: The transformed numerical values and the encrypted text are displayed.

## Additional Notes

- The project is a basic demonstration of matrix-based encryption and is not intended for real-world cryptographic security.
- The output includes intermediate steps for educational purposes, showing the numerical conversions and matrix transformations.
