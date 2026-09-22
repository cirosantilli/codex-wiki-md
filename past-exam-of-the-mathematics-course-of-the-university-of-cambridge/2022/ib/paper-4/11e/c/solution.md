<h1 id="11e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

[Gauss-Bonnet theorem](../../../../../../gauss-bonnet-theorem.md) gives the area of a curvature-$-1$ triangle as $\pi-(\alpha+\beta+\gamma)$. Split the regular polygon into $2n$ congruent right triangles. If $\theta$ is a polygon half-angle, the right-triangle identity and part (a) give

$$
\tan\theta
=\frac1{\tan(\pi/n)\cosh R}
=\frac{1-r^2}{1+r^2}\cot\frac\pi n.
$$

The polygon area is $(n-2)\pi-2n\theta$. Rewriting $\theta=\pi/2-\cot^{-1}(\tan\theta)$ yields

$$
\boxed{
A_n(r)=2n\left[
\cot^{-1}\!\left(\frac{1-r^2}{1+r^2}\cot\frac\pi n\right)
-\frac\pi n\right]}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11E](../../11e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
