Mixology with 1.9.1 compatibility
=================================

Mixology is a great C extension for Ruby that enables you to dynamically mix and unmix
modules from classes. Unfortunately the official version has not yet been updated to work with Ruby 1.9.1
and so I decided to try my hand at updating it myself. The 1.9.1 C API is not much different to 1.8.6, but
it does come with a bunch of macros that make using it a touch easier than 1.8.6.

The mixology.c file in this repo is modified to work with Ruby 1.9.1, it also works out of the box with Ruby 1.8.6.

To compile mixology.c for 1.9.1

* Run extconf.rb with the **Ruby 1.9.1 interpreter**
* Type 'make'
* Run the 1.9.1 test file (mixology_test19.rb) with the 1.9.1 interpreter

To compile mixology.c for 1.8.6

* Run extconf.rb with the **Ruby 1.8.6 interpreter**
* Type 'make'
* Run the 1.8.6 test file (mixology_test18.rb) with the 1.8.6 interpreter

Other Mixology19 features:
* Error checking (raises an exception if it is not given a valid module parameter)

## Acknowledgments:
Thanks to Pat Farley, anonymous z, Dan Manges, Clint Bishop for writing such a cool library.


Enjoy!


