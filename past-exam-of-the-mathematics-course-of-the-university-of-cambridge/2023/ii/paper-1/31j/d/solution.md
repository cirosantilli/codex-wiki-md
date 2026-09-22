<h1 id="31j/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Assume $\pi\in C$ and

$$
(x-\pi)^T(z-\pi)\leq0
$$

for every $z\in C$. Expanding the squared [euclidean distance](../../../../../../euclidean-distance.md) gives

$$
\begin{aligned}
\|x-z\|_2^2
&=\|(x-\pi)-(z-\pi)\|_2^2\\
&=\|x-\pi\|_2^2+\|z-\pi\|_2^2
  -2(x-\pi)^T(z-\pi)\\
&\geq\|x-\pi\|_2^2.
\end{aligned}
$$

**Hence $\pi$ minimizes the distance from $x$ over $C$, so $\pi=\pi_C(x)$. This proves the sufficient direction of the [variational characterization of convex projection](../../../../../../variational-characterization-of-convex-projection.md).**

## ↑ Ancestors (11)

1. [D](../d.md)
2. [31J](../../31j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
