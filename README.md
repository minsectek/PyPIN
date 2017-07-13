PyPIN
=
WARNING: This project is a work-in-progress!
PyPIN is a very simple Python module which can generate every possible 4-digit or 8-digit number, among a couple extra features. It got its name from its original use - generating sets of Bluetooth & 802.11 WPS PINs for an upcoming project. However, it can be used in a variety of ways - the sky's the limit!

Usage
=
To "install" the module, simply place it in the same directory as the script using it, or put it in your PYTHONPATH.
```
import PyPIN
# To output every number between 0 and 9999:

PyPIN.uptofour()

# Unfortunately, it's not currently possible to generate PINs starting with 0 (other than 0 itself...)

# To output every number between 1000 and 9999:

PyPIN.allfour()

# Same two things go for the generation of eight-digit PINs: "PyPIN.alleight" and "PyPIN.uptoeight" act the same as their four-digit counterparts.
```

Known bugs
=
The only currently-known bug is that, as mentioned above, it is currently not possible to generate any PIN beginning with 0, other than the number zero itself in "upto" functions. This is caused by the way Python (and most other languages, for that matter) handle integers. I am working on a way to bypass this without having to encode the PINs as strings.

Please do not use this module to brute-force credit card PINs.
=

