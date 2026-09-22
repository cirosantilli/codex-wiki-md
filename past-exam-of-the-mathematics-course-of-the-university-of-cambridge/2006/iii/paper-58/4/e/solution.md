<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

For $p=t=-1$, the preceding matrix becomes

$$
Q=\begin{pmatrix}\cos2\chi&\sin2\chi\\-\sin2\chi&\cos2\chi\end{pmatrix}_{(g,b)}.
$$

Multiplying it by $(\sin\chi,\cos\chi)^T$ gives $(\sin3\chi,\cos3\chi)^T$. The sine and cosine addition identities then prove by induction that

$$
\boxed{Q^r|\psi\rangle=\sin((2r+1)\chi)|g\rangle+\cos((2r+1)\chi)|b\rangle,\qquad
p_r=\sin^2((2r+1)\chi).}
$$

For $0<\chi\le\pi/4$, the first angle reaching the interval $[\pi/4,3\pi/4]$ gives success at least one half. Its smallest integer iteration count is

$$
\boxed{r_{1/2}=\left\lceil\frac{\pi}{8\chi}-\frac12\right\rceil
\sim\frac{\pi}{8}\sqrt{\frac Nm}\quad(m/N\to0).}
$$

The ceiling advances the angle by less than $2\chi$, so the chosen angle remains in that success interval. This is the [first half-success time in Grover search](../../../../../../first-half-success-time-in-grover-search.md). If near-certain rather than half success is desired, choose the nearest integer to $\pi/(4\chi)-1/2$; its success is at least $\cos^2\chi$ and the count is asymptotic to $(\pi/4)\sqrt{N/m}$. Both exhibit the quadratic query improvement of [amplitude amplification](../../../../../../amplitude-amplification.md). Success oscillates, so further iterations past the first maximum are not automatically beneficial. The count presumes positive known $m$ (or known $\chi$); if no marked item exists, no number of iterations can produce one.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
