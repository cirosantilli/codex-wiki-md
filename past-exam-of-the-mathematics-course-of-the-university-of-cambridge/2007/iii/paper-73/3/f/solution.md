<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

One limitation is finite useful storage capacity and interference. Under simple [Hebbian learning](../../../../../../hebbian-learning.md), each additional pattern contributes cross-talk to the retrieval fields; correlated or excessive patterns can erase a memory's basin or destabilize the pattern itself. More structured learning can reduce this interference: covariance-based weights account for activity biases, and pseudoinverse-based rules can orthogonalize a set of linearly independent patterns. Sparse representations and suitable thresholds can also change the capacity tradeoff. These extensions require their own retrieval analysis; they do not permit unlimited robust storage in a finite network.

A second limitation is spurious attractors and entrapment in unintended local minima. Mixtures of memories or unrelated configurations can be fixed points, and deterministic energy descent cannot escape an already stable incorrect state. Stochastic updates that sometimes accept energy increases can explore other configurations, and [simulated annealing](../../../../../../simulated-annealing.md) can gradually reduce that randomness to favor lower energies. Better weight learning and basin shaping can reduce the spurious states. Finite-temperature escape is probabilistic, and a practical finite-time annealing schedule does not guarantee the desired memory or a global minimum.

**Changing the learning rule addresses interference; changing the retrieval dynamics can address trapping.** The objective must still be appropriate: the lowest energy pattern is not necessarily the memory best matching a particular noisy cue.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
