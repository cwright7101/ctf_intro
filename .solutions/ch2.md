Options are essentially the same as ch1.md:

GDB, load binary in and set break point at main, start execution and once it starts the password is loaded onto the stack.

Ghidra, load in the binary to ghidra, go to main and you will see a string compare function with a password. after that it prints out what the actual password for this challenge is.

ltrace, ltrace ./ch2.bin will print out the strcmp with the password

strings, in this case the password is plain text string in the binary.

If you are on a linux machine, you can actually run this binary. The username is 'john'. Password is 'the ripper'. It will then print out the password string that we are looking for: '987654321'

