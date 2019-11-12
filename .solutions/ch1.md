Options:

GDB, load binary in and set break point at main, start execution and once it starts the password is loaded onto the stack.

Ghidra, load in the binary to ghidra, go to main and you will see a string compare function with a password.

ltrace, ltrace ./ch1.bin will print out the strcmp with the password

strings, in this case the password is plain text string in the binary.


password is: '123456789'