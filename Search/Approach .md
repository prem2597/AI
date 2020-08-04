# Approach

- Start with a frontier that contains the initial state
- Repeat :
    - if the frontier is empty, then there is no solution.
    - Remove a node from the frontier.
    - if node contains goal state, return the solution.
    - Expand node, add resulting nodes to the frontier.

# Reason for the revised approach 
- As in the previous approach if the node has has both forward and backward arrow like A<-->B then there might be a chance of infinite loop.

 
# Revised Approach

- Start with a frontier that contains the initial state.
- Start with an empty explored set.
- Repeat:
    - if the frontier is empty, then no solution.
    - Remove a node from the frontier.
    - if node contains goal state, return the solution.
    - Add the node to the explored set.
    - Expand node, add resulting nodes to the frontier if they aren't already in the frontier or the explored set.

