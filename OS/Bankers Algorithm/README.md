# Aim: 
To demonstrate Bankers Algorithm.

## Algorithm: 
Let ‘n’ be the number of processes in the system and ‘m’ be the number of resources types.
Available : 

It is a 1-d array of size ‘m’ indicating the number of available resources of each type.
Available[ j ] = k means there are ‘k’ instances of resource type Rj
Max :

It is a 2-d array of size ‘n*m’ that defines the maximum demand of each process in a system.
Max[ i, j ] = k means process Pi may request at most ‘k’ instances of resource type Rj.
Allocation :

It is a 2-d array of size ‘n*m’ that defines the number of resources of each type currently allocated to each process.
Allocation[ i, j ] = k means process Pi is currently allocated ‘k’ instances of resource type Rj
Need :

 It is a 2-d array of size ‘n*m’ that indicates the remaining resource need of each process.
Need [ i,   j ] = k means process Pi currently need ‘k’ instances of resource type Rj
for its execution.

Need [ i,   j ] = Max [ i,   j ] – Allocation [ i,   j ]



Allocationi specifies the resources currently allocated to process Pi and Needi specifies the additional resources that process Pi may still request to complete its task.

Banker’s algorithm consists of Safety algorithm and Resource request algorithm.

