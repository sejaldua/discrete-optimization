## Week 2: The Knapsack Problem

- What is "greedy"?
  - assume it's "easy" to build a feasible solution
  - build a solution by picking one item at a time
  - idea 1: more items is best, take small ones first until you run out of space
  - idea 2: valuable items is best, take valuable ones first until you run out of space
  - idea 3: value density, defined as dollars per kilogram
- for one problem, there are *many* possible greedy algorithms
  - some will do better than others
  - depends on the input!
- advantages
  - quick to design and implement
  - can be very fast
- problems
  - no quality guarantees (in general)
  - quality can vary widely on the input
  - problem feasibility needs to be "easy"