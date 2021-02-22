# hamiltonian-cycle-in-C
More practice coding in C (now with makefiles, utils, and headers oh my!)

This problem is framed as the following scenario:

A park ranger has to trim all the trees on a mountain slope. Since it is winter, the slope is covered in snow and it is not safe to climb it directly. Therefore, the ranger plans to chairlift to the top of the mountain and ski down the slope, trimming the trees as they go down. You are provided with a map of the trees on the ski slope with the possible routes between trees. You must write an algorithm to answer the following question: can the park ranger trim all of the trees using the chairlift only once? In other words, is there a single run the park ranger can perform from the top of the mountain which goes past every tree, or does the park ranger require multiple trips down the mountain?

Essentially, we are checking whether or not there's a hamiltonian path in a directed acyclic graph. If there are n trees and m edges between trees then the algorithm runs in O(n + m).

## input
- One line containing integers n and m. n indicates the number of trees, and m indicates the
number of possible routes (i.e., edges) between trees (or between the top of the mountain and a
tree).
- m lines containing two integers u and v, which indicates that it’s possible for the park ranger to
ski from u directly to v.
- The trees are labelled 1 to n, while the top of the mountain is always labelled 0.
