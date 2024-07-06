So you want to scale your application?
## Basic Concepts 
1) avoid state in your application, this makes everything easier to let other things hold your state (aka, think databases)
2) Scaling up is ok at the start... and for a LOT of applications
	1) 1 big beefy machine
3) Simple is easier to scale then complicated KISS

## Things that need to scale
CPU/Memory
Disk,
Network,
Complexity
## Basic Scaling tools
1) Load Balancing
2) Caching
3) Backoffs

## Medium Scaling tools
1) Metrics/observability of the system
2) Traceability
3) Coffee
4) Partitioning 
5) Load Shedding

## Seal Team 6 Scaling:

4) QoS
5) Networking
6) Event based systems
7) Nearline, "real time" systems
8) Batch Processing
9) Algorthims - Fan in/Fan out

### Locations that Tend to have issues

#### Database:
When a database is struggling to scale there many things you can do. 
(listed in order of amount of work)

 - A quick fix that requires "mostly no change" is to put a cache in front of it.
 - Many of the times you can update your indexes to match your access patterns better
	 - WARNING - you can make your database WORSE if you don't understand your data.
#### WARNING NOT RECOMMENDED UNLESS YOU CANT DO ANYTHING ELSE
 - you can redesign your database to better fit your data better 
 - Pick a database that "does" what you want to do better

