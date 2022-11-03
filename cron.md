the cron service allows us to schedule commands to run at regular intervals such as:

- every 30 mins
- every day at midnight
- every 1st of the month
- every december 15th
- etc.

https://crontab.guru/

to set up a cron job, need to edit the crontab configuration file. rather than edit the file directly, its best to use the crontab -e command (which will pull up the crontab file)

cron syntax

a b c d e command
minute hour day month day(of week)
0-59 0-23 1-31 1-12 0-6

for day(of week), 0 is sunday

- any value
  , list of values

* range of values
  \*/ step values
  */ step values 

  # adfh 
   --
   
