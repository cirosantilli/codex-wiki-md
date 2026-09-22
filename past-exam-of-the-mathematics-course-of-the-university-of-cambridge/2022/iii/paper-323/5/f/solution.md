<h1 id="5/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Assume an anti-degradable channel transmits perfectly with encoder $\mathcal E$ and decoder $\mathcal D$. Apply its Stinespring isometry to $\mathcal E(\rho)$, producing receiver system $Q$ and environment $E$. The receiver obtains $\rho$ by $\mathcal D$; anti-degradability lets the environment simulate the receiver output using $\mathcal N$, and then $\mathcal D\circ\mathcal N$ also produces $\rho$.

Apply these two local decoding channels simultaneously to $Q$ and $E$. Each marginal of the resulting bipartite state is the original pure state $\rho$. A bipartite state with a pure marginal is a product, so the joint output is $\rho\otimes\rho$. We have therefore constructed one quantum channel mapping every pure $\rho$ to $\rho\otimes\rho$, contradicting the [no-cloning theorem for two pure states](../../../../../../no-cloning-theorem-for-two-pure-states.md). Hence no anti-degradable channel can transmit arbitrary quantum information perfectly in one use.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [5](../../5.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
