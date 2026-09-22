<h1 id="13a/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write the function from the preceding part as $F_m$. Its expansion at zero is

$$
F_m(z)=-\frac12+z\left(\frac16-
\frac1{\pi^2}\sum_{k=1}^m\frac1{k^2}\right)+O(z^3).
$$

Hence the [residue theorem](../../../../../../residue-theorem.md) gives

$$
\frac1{2\pi i}\oint_{C_R}\frac{F_m(z)}{z^2}\,dz
=F_m'(0)=\frac16-\frac1{\pi^2}\sum_{k=1}^m\frac1{k^2}.
$$

Choose $R=R_m=(m+\tfrac12)\pi$. This circle stays a distance at least $\pi/2$ from every pole of $f$, so $f$ is bounded uniformly on it. Moreover

$$
\sum_{k=1}^m\left|\frac z{z^2+\pi^2k^2}\right|
\leq\sum_{k=1}^m\frac{R_m}{R_m^2-\pi^2k^2}
=O(\log m).
$$

Thus $\max_{C_{R_m}}|F_m|=O(\log m)$, and the [ML inequality](../../../../../../estimation-lemma.md) yields

$$
\left|\oint_{C_{R_m}}\frac{F_m(z)}{z^2}\,dz\right|
=O\left(\frac{\log m}{m}\right)\longrightarrow0.
$$

Letting $m\to\infty$ solves the [Basel problem](../../../../../../basel-problem.md):

$$
\boxed{\sum_{k=1}^{\infty}\frac1{k^2}=\frac{\pi^2}{6}.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [13A](../../13a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
