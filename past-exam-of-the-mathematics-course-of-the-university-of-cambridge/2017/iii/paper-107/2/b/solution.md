<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Here a domain is connected. Suppose both a negative point and a zero point exist. The open set $D=\{v<0\}$ then has a boundary point $q$ inside $\Omega$. Choose $z\in D$ close enough to $q$ that the [Euclidean ball](../../../../../../euclidean-ball.md) of radius $R=\operatorname{dist}(z,Z)$ stays compactly inside $\Omega$; it is contained in $D$ and touches $Z$ at some $y$. Attainment of this distance follows by restricting to a compact neighbourhood of $q$.

On that [Euclidean ball](../../../../../../euclidean-ball.md) $v$ is twice differentiable and

$$
\Delta v=-v>0,\qquad v(y)=0>v(x)\quad(x\in B_R(z)).
$$

The [Hopf boundary point lemma](../../../../../../hopf-lemma.md) gives a strictly positive outward radial derivative at $y$. But $y$ is an interior maximum of the $C^1$ function $v$ on $\Omega$, so $Dv(y)=0$. This contradiction proves the [Hopf dichotomy with classical regularity away from the zero set](../../../../../../hopf-dichotomy-with-classical-regularity-away-from-the-zero-set.md):

$$
\boxed{v\equiv0\quad\text{or}\quad v<0\text{ throughout }\Omega.}
$$

For the requested weaker-regularity counterexample take $\Omega=(-1,1)^n$ and

$$
\boxed{v(x)=-\max\{\sin x_1,0\}.}
$$

It is a [locally Lipschitz function](../../../../../../locally-lipschitz-function.md) and nonpositive. Its negative set is $x_1>0$, where $v=-\sin x_1$ is smooth and $\Delta v+v=0$. On $x_1\leq0$ it is zero. The [normal derivative](../../../../../../normal-derivative.md) jumps from zero to minus one across $x_1=0$, so it is not $C^1$. All other hypotheses hold; imposing the equation also across that interface would be an additional condition absent from the question.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
