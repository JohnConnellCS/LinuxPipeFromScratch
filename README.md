# UID: 506129117
# You Spin Me Round Robin

Given a set of input processes and a quantum length,
this program imitates "round robin" scheduling, outputting
the average wait and response times across the processes.

## Building

```shell
Run 'make' to build the executable
```

## Running

cmd for running './rr [path/to/processes/file.txt] [quantum_length]'
```shell
To run the command, specify the path to the processes file followed
by the quantum length. The txt file should be of the form:

numProcesses
processID1, arrivalTime, burstTime
processID2, arrivalTime, burstTime

repeated for each of the processes specified(see example). Say our 
txt file was stored in ./proc.txt and we wanted a quantum length of 8.
We would run 

'./rr proct.txt 8'

```

results 
SYNTAX:
'Average waiting time:
Average response time:'
```shell
Say we want to run the executable with some process file
proc.txt with the following contents:

4
1, 0, 7
2, 2, 4
3, 4, 1
4, 5, 4

This would indicate 4 processes with process ids, arrival times,
and burst times as indicated. If we wanted to run these 
processes with a quantum length of 3:

'./rr proc.txt 3'

which outputs

Average waiting time: 7.00
Average response time: 2.75

```

## Cleaning up

```shell
run 'make clean' to remove the executable made by make
```
