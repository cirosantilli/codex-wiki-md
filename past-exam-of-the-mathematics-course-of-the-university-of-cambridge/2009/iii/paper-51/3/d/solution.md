<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $\phi=j\pi/2$ for an integer $j$, and put $q=j\bmod2$. Use the fixed phase-measurement angles $(\theta,0,-\phi)$ and a fixed final [computational basis](../../../../../../computational-basis.md) measurement. Denote their outcomes by $k,l,m,s$. The adaptive construction would instead use $-\phi$ when $l=0$ and $+\phi$ when $l=1$.

For the printed measurement vectors,

$$
|v_t(\eta+j\pi)\rangle=|v_{t\oplus q}(\eta)\rangle.
$$

Therefore $+\phi$ and $-\phi$ define the same unordered pair of rank-one [linear projections](../../../../../../projection-linear-algebra.md); the labels are exchanged if and only if $q=1$. In the branch $l=1$, the outcome that would be called $m_{\mathrm{ad}}$ in the adaptive experiment is thus $m\oplus q$. In both branches,

$$
m_{\mathrm{ad}}=m\oplus ql.
$$

The output correction from the preceding part becomes

$$
\boxed{r=s\oplus k\oplus m\oplus ql.}
$$

If $j$ is even this reduces to $s\oplus k\oplus m$; if $j$ is odd an additional $l$ is included. This [equatorial measurement relabeling at Clifford angles](../../../../../../equatorial-measurement-relabeling-at-clifford-angles.md) changes only the classical interpretation, not any physical measurement basis.

All four fixed single-[qubit](../../../../../../qubit.md) [projective measurements](../../../../../../projective-measurement.md) act on different vertices, so their operators commute. They can be performed simultaneously, with the displayed classical correction applied afterward. The first angle $\theta$ may be arbitrary: it was never adaptive. Only the sign choice for the third angle needed to be replaced. Thus **the simulation is nonadaptive for every $\phi\in(\pi/2)\mathbb Z$**.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
