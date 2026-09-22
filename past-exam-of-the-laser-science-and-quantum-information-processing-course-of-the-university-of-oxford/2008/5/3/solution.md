<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $q=\cos^2(\pi/8)=(2+\sqrt2)/4$ and $1-q=\sin^2(\pi/8)$. In the [computational basis](../../../../computational-basis.md), input $|a\rangle$ has outcome probabilities $(q,1-q)$, while $|b\rangle$ has $(1-q,q)$. The marginal outcomes are equally likely; the [Bayesian posterior](../../../../bayesian-posterior.md) probabilities are

$$
\begin{array}{c|c|cc}
\text{outcome}&P(\text{outcome})&P(a\mid\text{outcome})&P(b\mid\text{outcome})\\\hline
0&1/2&q&1-q\\
1&1/2&1-q&q
\end{array}.
$$

Guess $a$ after zero and $b$ after one. Each guess is correct with probability **$q\simeq0.853553$** and wrong with probability **$1-q\simeq0.146447$**. Neither outcome is certain evidence for one input.

For a real state $|\psi_\theta\rangle=\cos\theta|0\rangle+\sin\theta|1\rangle$, the [Born rule](../../../../born-rule.md) in the [Hadamard basis](../../../../hadamard-basis.md) gives $P(\pm\mid\theta)=(1\pm\sin2\theta)/2$. Both angles $\pi/8$ and $3\pi/8$ have $\sin2\theta=1/\sqrt2$. Thus both preparations give $P(+)=q$ and $P(-)=1-q$. By [Bayes' theorem](../../../../bayes-theorem.md), **either outcome leaves the two input hypotheses equally likely**. The biased outcome frequencies carry no information about which state was prepared; the best success probability with this measurement is **$1/2$**.

## ↑ Ancestors (12)

1. [3](../3.md)
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
