Once upon a time, there was a logger named "John" with a job of sorting logs in a given directory. Then, some people decided to use the log program instead. This program took log files in a given directory, scanned the input, created indexes of its inputs, and printed out this index from a specified column (or line in the output file).

The program would print out log entries with a timestamp in the bottom right corner, starting with the last input file. The timestamp was of course an index into the log files, the index was a sequence of log entries starting with the timestamp.

So here is the first version of "John" (this is the standard text format):

print(log('Log Entry 1-20'));

print(log('Log Entry 2-20'));

print(log('Log Entry 3-20'));

print(log('Log Entry 4-25'));

print(log('Log Entry 5-20'));

print(log('Log Entry 6-20'));

print(log('Log Entry 7-20'));

print(log('Log Entry 8-20'));

print(log('Log Entry 9-20'));

print(log('LogEntry 10-20'));

print(log('Log Entry 11-20'));

print(log('LogEntry 12-20'));
