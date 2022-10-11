# Quartz Cron

## Cron Triggers
Cron-Expressions are strings that are actually made up of seven sub-expressions, 
that describe individual details of the schedule. 

These sub-expression are separated with white-space, and represent:

1. Seconds
2. Minutes
3. Hours
4. Day-of-Month
5. Month
6. Day-of-Week
7. Year (optional field)


Example would be 0 15 10 * * ? * – Fire at 10:15am every day. You can also use some special characters, listed few important ones below:

1. * every minute if * is placed in minute field
2. ? useful when you need to specify something in one of the two fields in which the character is allowed, but not the other.
3. – used to specify ranges.
4. , to specify additional values
5. / used to specify increments. For example, “0/15” in the seconds field means “the seconds 0, 15, 30, and 45″.


The following is another example, that triggers the job every other 10 seconds.

0/10 * * * * ? *