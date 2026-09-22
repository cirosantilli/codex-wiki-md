<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

[Weak convergence](../../../../weak-convergence.md) means $\ell(u_j)\to\ell(u)$ for every [bounded linear functional](../../../../continuous-linear-functional.md) $\ell\in X^*$. [Norm convergence](../../../../norm-convergence.md) implies this by $|\ell(u_j-u)|\leq\|\ell\|\|u_j-u\|$. The converse fails for coordinate unit vectors in $\ell^2$: their [norms](../../../../norm.md) are one, but pairing with any square-summable [sequence](../../../../sequence.md) tends to zero, so they are weakly null.

For the [subsequence](../../../../subsequence.md) assertion apply [Gram-Schmidt process](../../../../gram-schmidt-process.md) to a countable dense subset to choose a countable [orthonormal basis](../../../../orthonormal-basis.md) $(e_m)$ of the [separable Hilbert space](../../../../separable-hilbert-space.md) and a bound $M$ for the [sequence](../../../../sequence.md). Repeated [subsequence](../../../../subsequence.md) selection and diagonalization make every coefficient $\langle u_{j_k},e_m\rangle$ converge to a scalar $a_m$. [Bessel inequality](../../../../bessel-s-inequality.md) gives $\sum_{m=1}^N|a_m|^2\leq M^2$ for every $N$, so $u=\sum_ma_me_m$ exists in $H$ with [norm](../../../../norm.md) at most $M$. Pairings with finite [linear combinations](../../../../linear-combination.md) of the basis converge. Approximating any other test vector by such combinations and using the common [norm](../../../../norm.md) bound proves **$u_{j_k}\rightharpoonup u$**. The finite-dimensional case uses the same argument with a finite basis.

Apply this to every [subsequence](../../../../subsequence.md) of the bounded $L^2$ [sequence](../../../../sequence.md). Any [weakly convergent](../../../../weak-convergence.md) further [subsequence](../../../../subsequence.md) has limit $v$ with $\int_a^bv=0$, since interval indicators are $L^2$ tests. The permitted fact gives $v=0$ almost everywhere. If the whole [sequence](../../../../sequence.md) failed to converge weakly to zero, some fixed test functional and [subsequence](../../../../subsequence.md) would stay a positive distance from zero. Its [weakly convergent](../../../../weak-convergence.md) further [subsequence](../../../../subsequence.md) would then contradict the preceding conclusion. Thus **the entire [sequence](../../../../sequence.md) converges weakly to zero in $L^2(0,1)$**.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../split.md)
5. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
