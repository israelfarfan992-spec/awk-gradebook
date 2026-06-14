
## Task 1
Command: awk -F',' 'NR>1 {count++} END {print count}' Lab03-data.csv

Result: 322

Explanation: -F',' tells awk the file is comma-separated. NR>1 skips the header, count++ counts each submission, and END prints the final total


## Task 2
Command: awk -F',' 'NR>1 {seen[$1]=1} END {for (s in seen) count++; print count}' Lab03-data.csv

Result: 14

Explanation: NR>1 skips the header. The array seen[$1] stores each student name once, then the END loop counts how many different names were saved.
