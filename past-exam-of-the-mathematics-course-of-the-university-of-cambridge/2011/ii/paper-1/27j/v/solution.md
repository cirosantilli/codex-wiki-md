<h1 id="27j/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

A path that reaches level $c$ from below does so while in state $+1$, because $Z$ is continuous and has slope $X$. At the first crossing time, the residual exponential holding time is memoryless and the [Strong Markov property](../../../../../../strong-markov-property.md) restarts the chain from $+1$. Conditional on ever reaching $c$, the probability of subsequently exceeding $c+d$ is therefore exactly the original probability of exceeding $d$. Hence

$$
\psi_+(c+d)=\psi_+(c)\psi_+(d),\qquad\psi_+(0+)=1.
$$

The zero-level limit is one because the initial $+1$ holding time is positive almost surely. Also $0<\psi_+(c)\leq1$, and it is nonincreasing. Consequently $h(c)=-\log\psi_+(c)$ is nondecreasing and additive. First $h$ is linear on positive rationals, then monotonicity gives the same result on all positive reals. Thus

$$
\boxed{\psi_+(c)=e^{-Ac}\text{ for some }A\geq0.}
$$

Absorption can be viewed as killing at rate $\lambda$, independent of sign changes at rate $q$; this ensures the maximum is finite almost surely and makes the positive decay rate found in (iv) natural.

## ↑ Ancestors (12)

1. [V](../v.md)
2. [27J](../../27j.md)
3. [Section II](../../section-ii.md)
4. [Paper 1](../../../paper-1-split.md)
5. [Ii](../../../split.md)
6. [2011](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
