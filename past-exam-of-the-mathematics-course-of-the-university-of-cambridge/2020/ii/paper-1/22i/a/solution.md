<h1 id="22i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [continuous dual space](../../../../../../continuous-dual-space-split.md) of a real [normed vector space](../../../../../../normed-vector-space.md) $X$ is

$$
X^*=\{\phi:X\to\mathbb R:\phi\text{ is linear and bounded}\},
$$

with the [operator norm](../../../../../../operator-norm.md)

$$
\|\phi\|=\sup_{\|x\|\le1}|\phi(x)|.
$$

Two normed spaces are [isometrically isomorphic](../../../../../../isometric-isomorphism-of-normed-spaces.md) when there is a bijective linear map between them that preserves norms.

For $y=(y_j)\in\ell^\infty$, define

$$
\Phi_y(x)=\sum_{j=1}^{\infty}x_jy_j,
\qquad x\in\ell^1.
$$

The series is absolutely convergent and

$$
|\Phi_y(x)|\le\|y\|_\infty\|x\|_1,
$$

so $\Phi_y\in(\ell^1)^*$ and $\|\Phi_y\|\le\|y\|_\infty$. For every $\varepsilon>0$, choose $j$ with $|y_j|>\|y\|_\infty-\varepsilon$ and test on $\operatorname{sgn}(y_j)e_j$. This gives the reverse inequality, hence

$$
\|\Phi_y\|=\|y\|_\infty.
$$

Conversely, given $\Phi\in(\ell^1)^*$, set $y_j=\Phi(e_j)$. Then $|y_j|\le\|\Phi\|$, so $y\in\ell^\infty$. For $x\in\ell^1$, its finite partial sums converge to $x$ in norm; continuity of $\Phi$ therefore gives

$$
\Phi(x)=\lim_{N\to\infty}\sum_{j=1}^Nx_j\Phi(e_j)
=\sum_{j=1}^{\infty}x_jy_j=\Phi_y(x).
$$

The representing sequence is unique, and the construction is linear and norm preserving. Thus the [duality of l1 and l infinity](../../../../../../duality-of-l1-and-l-infinity.md) proves

$$
\boxed{(\ell^1)^*\cong\ell^\infty\quad\text{isometrically}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [22I](../../22i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
