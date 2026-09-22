<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The overlap $\langle0|+\rangle=1/\sqrt2$ is nonzero, whereas [perfect discrimination of pure states requires orthogonality](../../../../perfect-discrimination-of-pure-states-requires-orthogonality.md). Consequently no single-copy [quantum measurement](../../../../quantum-measurement-split.md) can identify both preparations with certainty. After a nondegenerate [projective measurement](../../../../projective-measurement.md), the [loss of preparation information after a nondegenerate projective measurement](../../../../loss-of-preparation-information-after-a-nondegenerate-projective-measurement.md) prevents further measurements from recovering the missing label: conditional on the first outcome, the post-measurement state is the same for every compatible initial hypothesis. Repeating the same basis gives that outcome again; changing basis probes the collapsed state. Fresh, independently prepared copies would be additional resources.

In the [computational basis](../../../../computational-basis.md), input $|0\rangle$ always gives zero and remains $|0\rangle$. Input $|+\rangle$ gives zero or one with probability $1/2$, leaving the corresponding basis state. Combining these likelihoods with equal prior [probabilities](../../../../probability.md), the [Bayesian update after a projective measurement](../../../../bayesian-update-after-a-projective-measurement.md) gives

$$
\begin{array}{c|c|cc}
\text{outcome}&P(\text{outcome})&P(\text{input }0\mid\text{outcome})&P(\text{input }+\mid\text{outcome})\\\hline
0&3/4&2/3&1/3\\
1&1/4&0&1
\end{array}.
$$

For example, [Bayes' theorem](../../../../bayes-theorem.md) gives $P(0\text{ input}\mid0\text{ outcome})=(1/2)/(3/4)=2/3$. **Outcome one certifies input $|+\rangle$; outcome zero is ambiguous.** Both inputs that give outcome zero leave exactly the same post-measurement state $|0\rangle$.

In the [Hadamard basis](../../../../hadamard-basis.md), input $|+\rangle$ always gives $+$, while input $|0\rangle$ gives $+$ or $-$ equally. Therefore

$$
\begin{array}{c|c|cc}
\text{outcome}&P(\text{outcome})&P(\text{input }0\mid\text{outcome})&P(\text{input }+\mid\text{outcome})\\\hline
+&3/4&1/3&2/3\\
-&1/4&1&0
\end{array}.
$$

**Outcome minus certifies input $|0\rangle$; outcome plus is ambiguous.** Guessing the more likely input after the ambiguous outcome gives success probability **$3/4$** for either of these two fixed-basis measurements.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [5](../../5-split.md)
3. [2008](../../split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
