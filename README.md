Made by Ian Campbell

order O(n)

This program divides the the random integer input by radix starting with the least value. 

input may be unspecified, but must be non negative numbers. can also be zero padded, will return nine zero pads.

this program reads in via STDIN. and sends output to STDOUT. (zero padded)

this program is especially good with large amounts of data because it skips insertion sort step. 

Example of how it works:

given random numbers: 12 43 11 10 94 35

our program looks at the last digit in each number and places the number in its respected "bucket" based off that digit.

so the first sort will look like this: 10 11 12 43 94 35

Notice how the last digits in the numbers are sorted. 0 1 2 3 4 5 

now the second loop occurs but sorts upon the second digit. 

second sort lools like this: 10 11 12 35 43 94

the numbers are now sorted. 

this works regardless of variation in number size. i.e. we coud sort: 102 988888 1 23 4578 etc. 

the program will loop through each digit(starting at the least significant digit: the 1's digit) and sort. then move to the ten's digit, then hundred's etc. each time keeping track of the newly sorted arrangment and modifing that new arrangment upon the next iteration.  