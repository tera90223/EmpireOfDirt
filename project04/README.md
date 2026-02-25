### Description


### Pseudocode

```python
10,000 Fragments
remove the redundant ones

CHoose first fragment
Init k-mer size
iterate through the fragments
    choose fragment
    split into kmers (make the debrujin graph)
    compare the two graphs
    If no overlapping:
        some condition?

```

### Successes


### Struggles

### Reflections

## Group lead (Eric Arnold):

## Group members (Jersha, Chantera):
Chantera: First, it was difficult to differentiate between what should be stored in the class's state vs when it should just be a local copy in the function. Since the algorithm removes edges, I had to be mindful about mutating `self.graph` vs the local copy of the graph. 

Another struggle I had concerned inputting the 10 million reads from the mouse genome.  Memory complexity issues  arose which we did not fully address uring implementation. After our class discussion, I realized we can use generators to stream reads without holding all the reads in memory, reducing memory overhead.

Lastly, I struggled with the concept that the read fragments do not statisfy balance conditions presentied by Eulerian path as k-mer multiplicity and uneven coverage violates that balance. Our implementation extracts path using the semi-balance conditions which we deemed more biologically appropriate.

### Generative AI appendix:
Generative AI was used to review reflection for grammatical clarity and minor syntax corrections.
