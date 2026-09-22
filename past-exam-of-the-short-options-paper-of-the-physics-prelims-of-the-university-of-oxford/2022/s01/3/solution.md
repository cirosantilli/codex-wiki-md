<h1 id="s01/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Singularities and cuts.** There are four [simple poles](../../../../simple-pole.md) $z_j=e^{i(\pi/4+j\pi/2)}$, $j=0,1,2,3$, because the roots of $1+z^4$ are simple and do not coincide with $\pm1$. At $z=\pm1$, the local behavior is a nonzero constant times $(z\mp1)^{-1/2}$: these are square-root [branch points](../../../../branch-point.md). Infinity is not a [branch point](../../../../branch-point.md); on either branch $f(z)=O(z^{-5})$, so it extends there with a zero of order five. Three valid choices of [branch cuts](../../../../branch-cut.md) are the segment $[-1,1]$, the two rays $(-\infty,-1]\cup[1,\infty)$ joined through infinity, or a semicircular arc joining $-1$ to $1$ and avoiding the [poles](../../../../pole.md). A circuit about either endpoint changes the sign, while a circuit about both endpoints does not.

**Branch and residues.** On $\mathbb C\setminus[-1,1]$, let $s(z)=\sqrt{z^2-1}$ be the branch with $s(z)/z\to1$ at infinity, and define $\sqrt{1-z^2}=-is(z)$. Its upper boundary value on $(-1,1)$ is positive. The [residue](../../../../residue.md) at a [simple pole](../../../../simple-pole.md) $z_j$ is

$$
\operatorname{Res}(f,z_j)=\frac{i}{4z_j^3s(z_j)}.
$$

For fully explicit values, put

$$
A=\sqrt{\frac{\sqrt2-1}{2}},\qquad B=\sqrt{\frac{\sqrt2+1}{2}}.
$$

In counterclockwise order $z_0,z_1,z_2,z_3$, the values of $s$ are $A+iB,-A+iB,-A-iB,A-iB$. Since $A^2+B^2=\sqrt2$, substitution yields

$$
\boxed{\begin{aligned}
r_0=r_2&=\tfrac18\bigl[A-B-i(A+B)\bigr],\\
r_1=r_3&=\tfrac18\bigl[B-A-i(A+B)\bigr].
\end{aligned}}
$$

A [branch point](../../../../branch-point.md) has no ordinary [residue](../../../../residue.md), since it has no single-valued [Laurent series](../../../../laurent-series.md) on a punctured neighborhood. At infinity the [residue](../../../../residue.md) is zero.

**Contour evaluation.** The original contour goes counterclockwise around a large circle and clockwise round the slit, with its upper lip directed to the right. The large-circle contribution is $O(R^{-4})$. Small endpoint arcs contribute $O(\epsilon^{1/2})$. The artificial slit extension from $1$ to $R$ has equal boundary values on both sides, so its contributions cancel. On $(-1,1)$ the two boundary values of $f$ are opposite. Thus, with $I$ denoting the requested real integral, the [residue theorem](../../../../residue-theorem.md) gives

$$
2I=2\pi i\sum_{j=0}^3r_j,\qquad \sum_{j=0}^3r_j=-\frac{i}{2}(A+B).
$$

Therefore

$$
\boxed{I=\frac{\pi}{2}(A+B)=\frac{\pi}{2}\sqrt{1+\sqrt2}.}
$$

## ↑ Ancestors (12)

1. [3](../3.md)
2. [S01](../../s01.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../split.md)
5. [Short options paper of the physics Prelims of the University of Oxford](../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
