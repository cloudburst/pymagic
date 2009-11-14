# pymagic

[`pymagic`] is a simple Python wrapper for libmagic 

## Usage:

    git clone git://github.com/cloudburst/pymagic.git

    >>> from pymagic import *

    >>> libmagic.guess_file('/usr/bin/gcalctool')
    /usr/bin/gcalctool: ELF 64-bit LSB executable, x86-64, version 1 (SYSV), dynamically linked (uses shared libs), for GNU/Linux 2.6.15, stripped

    >>> libmagic.guess_string('PK\x03\x04\x00')
    'Zip archive data'

   >>> libmagic.find_in_file('/bin/rm')
    0x0: ELF 64-bit LSB executable, x86-64, version 1 (SYSV)
    0x7400: COM executable for DOS 
