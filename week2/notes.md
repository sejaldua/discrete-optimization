## Week 2: The Knapsack Problem

### Greedy Algorithm

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
- summary
  - we can always start with greedy
  - going beyond the greedy solution
    - constraint programming
    - local search
    - mixed integer programming

### Modeling

- Step 1: formalize an optimization task as a mathematical model
- the (1-dimensional) knapsack problem
  - given a set of items $I$, each item $i \in I$ characterized by
    - its weight $w_i$
    - its value $v_i$
    - capacity $K$ of knapsack
  - find the subset of items in $I$
    - that has maximum value
    - does not exceed capacity $K$ of the knapsack 
- Optimization Modeling
  - decision variables
    - *typically encode the result that we are interested in*
    - e.g., for a particular item, do we select it or not select it?
  - problem constraints
    - *specify what the feasible solutions to the problem are*
  - objective function
    - *specifies the quality of each solution*
- the result is an optimization model
  - it is a declarative formulation
    - specifies the "what", not the "how"
  - there may be many ways to model an optimization problem