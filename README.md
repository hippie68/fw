# fw
Simple Bash script that shows PS4 PKGs' SDK version and required firmware. 
Requires Bash script "sfo" (https://github.com/hippie68/sfo) in $PATH.

Usage:

    fw [options] [file|directory ...]
    
Options:

    -h  Display help
    -r  Traverse directories recursively

Example output:

    $ fw
    SDK:    FW:     File name:
    7.00	7.00    The Last of Us Part II [Game] [CUSA10249].pkg
    5.05	7.00    The Last of Us Part II [Update v1.07] [CUSA10249].pkg

Explanation:
- SDK: You can, theoretically, run the game if your real firmware version is equal or higher.
- FW: You can run the game if your real firmware version is equal or higher OR if you spoof your firmware version.  
Both conditions, for SDK and FW, must be met.
In the depicted, theoretical example, the update PKG is obviously backported. If your real firmware is lower than 7.00 you can run the game after you installed the patch and spoofed your firmware version (which recent HENs do automatically).

DLC has no firmware requirements.
