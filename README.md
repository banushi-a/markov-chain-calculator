# markov-chain-calculator
A Jupyter Notebook Project To Automate Common Markov Chain Calculations

## Goals:
We wish to differentiate between different kinds of Markov Chains, including:
1. Ergodic
2. Regular
3. Absorbing

Distinguishing ergodic Markov chains ended up being more complicated than the others. The approach we took was to consider the Markov chain as a graph, consisting of edges and nodes. Then by applying Tarjan's Algorithm, we could ascertain if the given graph consisted of a single strongly connected component. If it did, we found that we could reach any node from any other node in the graph, i.e. we could reach any state from any other state in the Markov chain. 

## Questions to Answer:
General questions we could answer are:
1. ✅ Probability to go from state **a** to state **b** in **k** steps
2. ✅ Average number of times in a state before being absorbed
3. ✅ Average number of steps before being absorbed
4. ✅ Probability that we are absorbed by state **b** if we start in state **a** (be absorbed)
5. ✅ Find the fixed vector of a matrix
6. ✅ Mean First Passage Time of ergodic matrix
7. ✅ Mean first return time for state **a**

In the current version, functions to answer each of these have been implemented and tested for correctness.

## Interactive Calculator

At the bottom of the notebook, a REPL style calculator has been implemented. If this were to be developed furhter, we may decide to treat the functions as a separate project, instead opting to develop some API. Doing so would allow for use in other languages and mediums, such as an interactive website for example.
