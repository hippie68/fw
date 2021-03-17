# fw
Simple Bash script that shows PS4 PKGs' required firmware.  
Requires Bash script "sfo" (https://github.com/hippie68/sfo) in $PATH.

Usage:

    fw [options] [file|directory ...]
    
Options:

    -h Display help
    -r Traverse directories recursively

Example output:

    $ fw
    FW:     File name:
    7.00	The Last of Us Part II [Game] [CUSA10249].pkg
    5.05	The Last of Us Part II [Update v1.07] [CUSA10249].pkg

Notes:
DLC has no firmware requirements.
