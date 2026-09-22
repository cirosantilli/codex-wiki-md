<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

With identity hidden activations and no biases, the pre-softmax map is a product of weight matrices. For any nonzero scalar $c$, multiplying the incoming weights of one hidden neuron by $c$ and dividing its outgoing weights by $c$ leaves that product, every output probability, and the cross-entropy unchanged. Every minimizer therefore belongs to an infinite continuum of equivalent parameterizations; more generally, invertible changes of hidden coordinates and their inverse in the adjacent layer give the same network function.

I would use `batch_size=1`. The resulting stochastic-gradient noise helps move along flat nonidentifiable directions and escape saddle regions, whereas full-batch gradient descent is deterministic and can stagnate in this highly nonconvex, singular parameterization.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
