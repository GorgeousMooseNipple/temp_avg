## Why
I wrote this script to see if my laptop cooling pad is making any difference in terms of cores' temperature.  
It does for a couple of degrees.  
This script essentially uses `sensors` utility, logs its output in a file and on exit with SIGINT or SIGTERM, calculates mean, max and min temperatures for each core, prints it in console and saves results in a log file. Or, with -q option set, just prints continuous measurements in console, just like `watch sensors` would.
### Options
-d - delay between measurements in seconds, 30 seconds by default  
-q - don't create log file, just continuously print current temperatures in console  
-m \<string\> - puts \<string\> in the name of a log file
