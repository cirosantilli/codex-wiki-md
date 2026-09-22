<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The two cusps of $\Gamma_1(2)$ are infinity and zero. At infinity,

$$
j(\tau)=q^{-1}+744+O(q),
\qquad
j(2\tau)=q^{-2}+744+O(q^2),
$$

so

$$
f(\tau)=\frac{j(\tau)}{j(2\tau)}=q+O(q^2).
$$

Thus $f$ is holomorphic at infinity and has a simple zero there.

Use the scaling matrix

$$
S=\begin{pmatrix}0&-1\\1&0\end{pmatrix}
$$

at the cusp zero. Since $j(-1/\tau)=j(\tau)$,

$$
(f|_0S)(\tau)
=\frac{j(-1/\tau)}{j(-2/\tau)}
=\frac{j(\tau)}{j(\tau/2)}.
$$

The width of zero is two, so its local parameter is $q_0=e^{\pi i\tau}$. As $\operatorname{Im}\tau\to\infty$,

$$
j(\tau)=q_0^{-2}+O(1),
\qquad
j(\tau/2)=q_0^{-1}+O(1),
$$

and therefore

$$
(f|_0S)(\tau)=q_0^{-1}+O(1).
$$

It has a simple pole at zero and is not holomorphic there. This uses the [width of a cusp](../../../../../../width-of-a-cusp.md) to express the two expansions in their correct local parameters.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
