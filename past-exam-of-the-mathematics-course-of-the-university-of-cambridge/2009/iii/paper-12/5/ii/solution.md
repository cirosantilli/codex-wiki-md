<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A local form of the [Harnack inequality for harmonic functions](../../../../../../harnack-inequality-for-harmonic-functions.md) is: if $u\geq0$ is harmonic on a neighbourhood of $\overline{B_{4r}(y)}$, then

$$
\boxed{\sup_{B_r(y)}u\leq3^n\inf_{B_r(y)}u.}
$$

For $x,z\in B_r(y)$, the triangle inequality gives $B_r(x)\subset B_{3r}(z)\subset B_{4r}(y)$. The ball [mean value property for harmonic functions](../../../../../../mean-value-property-for-harmonic-functions.md) and nonnegativity therefore imply

$$
u(x)=\frac1{|B_r|}\int_{B_r(x)}u\leq\frac1{|B_r|}\int_{B_{3r}(z)}u=\frac{|B_{3r}|}{|B_r|}u(z)=3^nu(z).
$$

Taking the supremum over $x$ and infimum over $z$ proves the inequality, including the case where the infimum is zero. No strict positivity assumption was used.

On a connected domain $\Omega$, the equivalent compact-set statement is that for each nonempty compact $K\Subset\Omega$ there exists $C(K,\Omega,n)$ with

$$
\boxed{\sup_Ku\leq C(K,\Omega,n)\inf_Ku.}
$$

Here is the passage from balls to this statement. Cover $K$ by finitely many small balls $B_{r_j}(y_j)$ whose quadrupled closed balls lie in $\Omega$. Join their centres to a fixed centre by paths in $\Omega$. Each of the finitely many paths has compact image and positive distance from the boundary, so subdividing it gives a finite chain of overlapping small balls whose quadrupled closures also lie in $\Omega$. The local inequality compares any two points in each ball; using a point in each successive overlap propagates comparisons along the chain. The number of comparisons is bounded uniformly over this finite collection of chains and covering balls. Multiplying the factors $3^n$ gives one finite constant for all pairs $x,z\in K$, proving the compact-set inequality. In particular a nonnegative harmonic function vanishing at one interior point vanishes throughout a connected domain.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
