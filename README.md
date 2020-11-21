# csci596_final_project

# Flow Computation Framework scheduler

## Problem
For the current flow computation, the computation DAG has to be well defined. 

However when the number of computers increasing, it wourl become harder and harder to schedule the resources. 

![Image of DAG](https://static001.infoq.cn/resource/image/96/e7/96d716aab379642b4d7e2c39ced658e7.jpg)
## Assumption
In a highly unstable network of computing nodes, the cost of communication would be high and various. 

By introducing a self envolving network DAG, we could release the main node from much scheduling job. 

![Image of flow network](https://upload.wikimedia.org/wikipedia/commons/a/ae/Network_flow_residual_SVG.svg)

## Steps
For each computing node we extract the information of the devices:


CPU GPU FPGA Memory output latency 

for each network connection, we extract the information of latency and possibility of network jam. 

Created a DAG which could evolve accordingly. 

Dynamically allocated different resources to different node and allocate different time tollerented. 

## Expected Result
It would make fault torrlence much easier to handle. 
For computing node with much different latency and power, it would not be identified as lost connection. 

