<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $k=b/a>1$ and $\mathbf e_z=(0,0,1)$. The complete construction of [image charges between concentric grounded spheres](../../../../../image-charges-between-concentric-grounded-spheres.md) consists of two families, indexed by every integer:

$$
\boxed{\begin{aligned}
q_n&=qk^n,&\mathbf r_n&=r_0k^{2n}\mathbf e_z,\\
\widetilde q_n&=-\frac{qa}{r_0}k^n,&\widetilde{\mathbf r}_n&=\frac{a^2}{r_0}k^{2n}\mathbf e_z,
\qquad n\in\mathbb Z.
\end{aligned}}
$$

The term $(q_0,\mathbf r_0)$ is the physical [point charge](../../../../../point-charge.md); every other term is an [image charge](../../../../../image-charge.md). In the first family $n\leq-1$ lies inside $r=a$ and $n\geq1$ lies outside $r=b$. In the second family $n\leq0$ lies inside $r=a$ and $n\geq1$ lies outside $r=b$. Thus no [image charge](../../../../../image-charge.md) lies in the physical gap.

To derive and verify these families, reflection of an axial [point charge](../../../../../point-charge.md) $(Q,z)$ in a grounded sphere of radius $R$ replaces it by the [image charge](../../../../../image-charge.md) $(-RQ/z,R^2/z)$. Reflection in $a$ sends $(q_n,\mathbf r_n)$ to $(\widetilde q_{-n},\widetilde{\mathbf r}_{-n})$; reflection in $b$ sends it to $(\widetilde q_{1-n},\widetilde{\mathbf r}_{1-n})$. Successive reflections therefore generate exactly the listed families. The [method of images](../../../../../method-of-images.md) gives

$$
\boxed{\phi(\mathbf r)=\frac1{4\pi\epsilon_0}\sum_{n\in\mathbb Z}
\left(\frac{qk^n}{|\mathbf r-r_0k^{2n}\mathbf e_z|}
-\frac{(qa/r_0)k^n}{|\mathbf r-(a^2/r_0)k^{2n}\mathbf e_z|}\right),\qquad a<r<b.}
$$

The physical [point charge](../../../../../point-charge.md) itself is excluded when evaluating this formula. On $r=a$, pair the first-family term $n$ with the second-family term $-n$; their [electric potentials](../../../../../electric-potential.md) cancel by the single-sphere distance identity. On $r=b$, pair $n$ with $1-n$ instead. These reindexings are justified by [absolute convergence](../../../../../absolute-convergence.md), as follows.

For $n\to-\infty$, both source positions tend to the origin while their [electric charges](../../../../../electric-charge-split.md) have size $O(k^n)$. On the closed gap their distances are eventually at least $a/2$, so both [electric potential](../../../../../electric-potential.md) terms are $O(k^n)$. For $n\to+\infty$, both distances are at least a positive constant times $k^{2n}$ and the [electric charges](../../../../../electric-charge-split.md) are $O(k^n)$, giving $O(k^{-n})$ terms. Both tails are bounded by convergent [geometric series](../../../../../geometric-series.md). This proves [absolute convergence](../../../../../absolute-convergence.md) and [uniform convergence](../../../../../uniform-convergence.md) of the tails on the closed gap. On any compact set avoiding the physical [point charge](../../../../../point-charge.md), the differentiated tails obey the same type of bounds: for example, the large positive tail of the [electric field](../../../../../electric-field-split.md) is $O(k^{-3n})$. Thus termwise differentiation is valid and the sum is a [harmonic function](../../../../../harmonic-function.md) except at the physical [point charge](../../../../../point-charge.md), where it has the correct [Coulomb's law](../../../../../coulomb-s-law.md) singularity. The boundary cancellations and [uniqueness of Poisson equation](../../../../../uniqueness-of-poisson-equation.md) complete the construction.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the electromagnetism course of the University of Oxford](../../../../split.md)
6. [Electromagnetism course of the University of Oxford](../../../../../electromagnetism-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
