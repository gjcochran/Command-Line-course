the cron service allows us to schedule commands to run at regular intervals such as:

- every 30 mins
- every day at midnight
- every 1st of the month
- every december 15th
- etc.

https://crontab.guru/ [helps verify if syntax is correct for cronjob cadence]

to set up a cron job, need to edit the crontab configuration file. rather than edit the file directly, its best to use the crontab -e command (which will pull up the crontab file)

# cron syntax
a b c d e command

a -- minute 0-59    
b -- hour 0-23
c -- day 1-31
d -- month 1-12
e -- day(of week) 0-6

- for day(of week), 0 is sunday

dash(-) ... any value [ie all, ex every day]
comma (,) ... list of values
asterick (*) range of values
asterickslash (*/) step values [ex. every 5]

exs. 
run a job at minute 30 (every time the clock shows 30 in the minutes position), ie. every hour 
30 * * * * command 

ex2. 
run a job every day at midnight
0 0 * * * command 

ex3. 
run a job every monday at 6:30am 
30 6 * * 1 command 

ex4. 
run a job every monday in april at 6:30am 
30 6 * 4 1 command 

ex5. 
run a job at midnight on the first of every month
0 0 1 * * command 

ex6. 
run a job at mightnight every weekday
0 0 * * 1-5 command

ex7. 
run a job every 5 minutes, in perpetuity
*/5 * * * * command 


# errors 

cronjobs dont by default tell you if there was an error, unless designate a place to redirect errors to 
with ex. 2>&1 (will redirect errors to the same log file)


MADE A TAR BALL related to making a backup of Desktop every day but did not fully set it up as did not add a schedule to this in crontabs.. for future reference in case do decide at some point to have backups run on regular cadence

