## Task 1
Command: awk -F',' 'NR>1 {count++} END {print count}' Lab03-data.csv

Result: 322

Explanation: -F',' tells awk the file is comma-separated. NR>1 skips the header, count++ counts each submission, and END prints the final total
