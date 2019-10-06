This problem functions on lsb (Least Significant Bit) Steganography. When you look at a byte, you commonly see a byte aligned like this:

11100101

The byte goes from "most significant bit" to least significant bit.
LSB Steganography takes advantage of the fact that changing the least significant bit by 1 does not change the number very much.
Allow me to demonstrate.

he number 255 in bytes is 11111111.
If we change the first bit to a zero, we get 01111111, which is 127. Changing the first byte subtracted 128.
However, if we change the last bit, we get 11111110, or 254. In comparison to changing the first bit, we get a much more similar
number to 255.

The image "cup.png" has another image hidden with LSB. The image is a 3bit image, meaning that its rgb values can be one of 2 values: on or off.
This makes it easy to hide in an RGB image, as the data for a pixel for the flag image could be stored perfectly in that data for a pixel for the
cup image.


