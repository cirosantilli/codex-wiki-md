<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each $n$, define $Jx_n:X^*\to\mathbb R$ by $Jx_n(f)=f(x_n)$. Weak convergence makes $(Jx_n(f))_n$ bounded for every $f\in X^*$. The [Uniform boundedness principle](../../../../../../uniform-boundedness-principle.md) gives

$$
\sup_n\lVert Jx_n\rVert=\sup_n\lVert x_n\rVert<\infty.
$$

Let $K$ be the closed convex hull of the $x_n$. Given a sequence in $K$, approximate its terms in norm by finite convex combinations of the $x_n$. A diagonal subsequence makes every coefficient converge. Any loss of total coefficient mass is assigned to zero, which belongs to $K$ by [Mazur theorem](../../../../../../mazur-theorem.md) because $x_n\rightharpoonup0$. Since $f(x_n)\to0$ for every $f\in X^*$, splitting each sum into a finite head and a uniformly small tail proves weak convergence of this subsequence to the corresponding convex combination. Hence $K$ is weakly sequentially compact and, by the stated theorem, weakly compact.

Define

$$
T:X^*\to c_0,
\qquad
Tf=(f(x_n))_{n\geq1}.
$$

It is bounded because $(x_n)$ is norm bounded, and its values lie in $c_0$ because $x_n\rightharpoonup0$. Its adjoint-on-preduals map is

$$
T_*:\ell^1\to X,
\qquad
T_*(a)=\sum_na_nx_n.
$$

If $K$ had nonempty norm interior, then $K-K$ would contain a ball about zero. The quantitative open-mapping argument applied to the convex combinations above would make $T_*$ surjective, and hence make $T$ bounded below. Its range $R$ would be a closed infinite-dimensional subspace of $c_0$ whose unit ball is compact for coordinatewise convergence, since it lies in the coordinatewise compact image of a weak-star compact ball of $X^*$.

By the stated structural theorem, $R$ contains a closed subspace isomorphic to $c_0$. The bounded partial sums of the image of the standard $c_0$ basis would then have a coordinatewise convergent subnet. Uniform boundedness turns coordinatewise convergence in $c_0$ into weak convergence, and norm-closed subspaces are weakly closed. Pulling the limit back would make the partial sums of the standard basis converge weakly in $c_0$, impossible because their coordinate values force the putative limit to be the constant-one sequence. This contradiction proves that $K$ has empty norm interior.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
