# perfect-tools
Linux micro tools for system administrators

## locker

"locker" make guarantee to single execution instance of your command. This is usable for CRON tasks and other.

Example execution:

    locker ping 8.8.4.4

Example cron-task:

    * * * * * root locker /any/your/script

## pingtop

"pingtop" is a tool for ping many hosts and display it on realtime. Example of screen:

    Mon Oct 31 15:23:16 MSK 2016
    10.10.0.1 	--> ...............
    10.10.0.2 	--> ....!....!.....
    10.10.0.100 	--> ...............
    10.10.1.1 	--> ...............
    10.10.1.12 	--> ..!..!..!..!...
    10.10.1.14 	--> ............!..
    10.10.251.1 	--> ...............
    10.10.252.2 	--> !!!!!!!!!!!!!!!
    10.10.3.1 	--> ...............
    10.10.3.3 	--> ...............

Example of usage:

    pingtop 10.10.0.1 10.10.0.2 10.10.0.100

or

    pingtop ip-per-row.txt

