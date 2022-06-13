What are checksums and what are they useful for?
Checksums are used for verification and to check data for errors.
Checksums are created using an algorithm, usually MD5, SHA-1, or SHA-256. Others can be used.
They are useful to help verify code or data if it has been altered.
Any piece of data can be run through an algorithm to get a checksum, which will be given a unique string of letters and numbers.
Using a checksum will help determine that the code is correct and without errors from its source.
Checksum can also be used for continuous data transfers.
In on of my projects, the lidar continously sent data. To determine when a new set of data was delivered, a checksum was used to separate values.
This is another form a checksum can be used. A specifc string of digits/characters to determine the end of a set of data.
