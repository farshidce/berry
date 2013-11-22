choosing a key value database with map/reduce capabilities

entities:

- node
- application
- stats related to an application that is running on a node
- group of nodes forming a cluster ?
- test run ?


- every sample : 
stat name. start time. end time

metadata:
name
start time
nodes


node:
ip
name
applications

application
name
heartbeats
path
args
pids

metric
name
unit
time
value
source(which is a node)


choose which test runtime

send stats to the server cotinously
update the database right away
query the database and send the data back to the UI

process view
process
stats for this process ?
memory? cpu? swap? cputime? ..

views : stats where process name = x and test-runtime = t ( does that mean for eevery new test run we have to create a new index ? )

indexes : 
