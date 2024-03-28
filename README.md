# The KL algorithm improves the bipartition iteratively by swapping pairs of nodes between the two sets. The nodes are exchanged in the order defined by their net gain, The cells with the highest gain are swapped first.
Although the KL algorithm cannot guarantee that it will find the optimal bipartition, it frequently produces high-quality solutions in practice. The KL algorithm requires multiple runs with different initial partitions may be required to obtain a good solution.
Kernighan Lin follows this approach
Begin by dividing the graph into two parts.
Calculate the net gain in edge weight for each node 
The difference between the number of edges going between the two sets and the number going within each set
Sort the nodes such that their gain is decreasing
Swap the first two nodes from the sorted list between the two sets.
Calculate the net gain for each affected node again.
These Steps should be repeated until no further improvement is possible.
Return the final division.
Algorithm used:
Kernighan Lin Algorithm used in the program:
Step1: Read in net-list file.
Step2: Create adjacency matrix.
Step3: Calculate cutset between two partitions.
Defining Kernighan-Lin algorithm:
------------------------------------------------------------------------------------------------------------
Step4: Initialize two partitions of equal size.
Step5: Calculate the gain for cell i moving from one partition to the other.
Step6: Iterate until no further improvement can be made or until max iterations is reached.
Step7: Calculate the gain for each cell in one partition moving to the other partition.
Step8: Move cells with highest gain to other partition.
Step9: Calculate new cutset.
Step10: Check if cutset has been minimized.
------------------------------------------------------------------------------------------------------------
Step11: Read in netlist.
Step12: Run Kernighan-Lin algorithm.
Step13: write output.
