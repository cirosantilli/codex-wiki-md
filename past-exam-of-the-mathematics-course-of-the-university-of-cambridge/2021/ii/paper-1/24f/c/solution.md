<h1 id="24f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Lift $u$ through the [complex exponential](../../../../../../exponential-function.md) by setting

$$
v(w)=u(e^w),\qquad w\in\mathbb C.
$$

The [conformal invariance of harmonicity](../../../../../../conformal-invariance-of-harmonicity.md) makes $v$ harmonic. Since $e^{w+2\pi i}=e^w$ and $u(2z)=u(z)$,

$$
v(w+2\pi i)=v(w),
\qquad
v(w+\log2)=v(w).
$$

Thus $v$ is bounded on the compact rectangle

$$
\{s\log2+2\pi it:0\leq s,t\leq1\},
$$

and its two [periods](../../../../../../period-lattice.md) make it bounded on the whole plane. The [harmonic Liouville theorem](../../../../../../harmonic-liouville-theorem.md) makes $v$ constant. Since the exponential map is surjective onto $\mathbb C^*$, $u$ is constant.

For the requested counterexample after deleting a countable set, take

$$
S=\{2^m:m\in\mathbb Z\}
$$

and let $\wp_\Lambda$ be the [Weierstrass elliptic function](../../../../../../weierstrass-elliptic-function.md) for the lattice

$$
\Lambda=(\log2)\mathbb Z+2\pi i\mathbb Z.
$$

Define

$$
u(z)=\operatorname{Re}\wp_\Lambda(\log z),
\qquad z\in\mathbb C^*\setminus S.
$$

Changing a branch of the logarithm adds $2\pi i$, a period of $\wp_\Lambda$, so $u$ is well defined. Its poles project precisely to $S$, and the [conformal invariance of harmonicity](../../../../../../conformal-invariance-of-harmonicity.md) makes $u$ harmonic away from them. The other period gives

$$
u(2z)=\operatorname{Re}\wp_\Lambda(\log z+\log2)=u(z).
$$

Moreover, $z\notin S$ implies $2z\notin S$. Finally, $u$ is nonconstant because as positive real $z\to1$,

$$
\wp_\Lambda(\log z)\sim\frac1{(\log z)^2},
$$

which is real and unbounded. This is a [scale-periodic harmonic function from an elliptic function](../../../../../../scale-periodic-harmonic-function-from-an-elliptic-function.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [24F](../../24f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
