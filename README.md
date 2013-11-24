EDC's Fork of PHPApacheLogViewer
==================
This fork is our attempt at addressing some the issues of PHPApacheLogViewer by fixing bugs and doing other dev stuff with the specific goal of supporting our usage of it.

### Changes ###
* ```index.php```: Fixes a bug that occurs when the log file is inaccessible or does not exist which causes PHPApacheLogViewer to get stuck in an infinite loop and floods your log file.

* ```index.php```: Added a setting ```$time_to_quit``` in the config file where you can specify for this script the max time limit. This is useful to force terminating the script if it is taking too long, which is a case you probably will experience if your logs are hefty. ```$time_to_quit``` defaults to 10 seconds.
