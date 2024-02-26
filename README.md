## Why
I wrote this script to see if my laptop cooling pad is making any difference in terms of cores' temperature.  
It does for a couple of degrees.  
This script essentially uses `sensors` utility, logs its output in a file while continuously printing current measurements in a console and on exit with SIGINT or SIGTERM, calculates mean and max temperatures for each core, prints results in a console and saves it in a log file. Or if -q option is set, just prints continuous measurements to a console, just like `watch sensors` would. It stores log files in the same directory where script is located in a specifically created folder.  
### Options
-d - delay between measurements in seconds, 30 seconds by default  
-q - don't create a log file, just continuously print current temperatures to a console  
-m \<string\> - puts \<string\> in the name of a log file
