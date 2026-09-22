# Singular value

↑ **Parent:** [Singular value decomposition](singular-value-decomposition.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Singular_value)

The [singular values](singular-value.md) of a [matrix](matrix.md) measure stretching of [Euclidean norm](euclidean-norm.md). They are the nonnegative [square roots](square-root.md) of the [eigenvalues](eigenvalue.md) of $A^*A$, counting the $\min(m,n)$ diagonal slots of the [singular value decomposition](singular-value-decomposition.md); when $n>m$, $A^*A$ has additional zero [eigenvalues](eigenvalue.md). Nonnegativity follows from $x^*A^*Ax=\|Ax\|_2^2\geq0$, so $A^*A$ is a [positive semidefinite matrix](positive-semidefinite-matrix.md). For the preceding $2\times2$ [matrix](matrix.md),

$$
A^TA=\frac1{25}\begin{pmatrix}241&288\\288&409\end{pmatrix},\qquad
AA^T=\begin{pmatrix}25&0\\0&1\end{pmatrix}.
$$

Both have [eigenvalues](eigenvalue.md) $25,1$, giving [singular values](singular-value.md) $5,1$. In particular,

$$
\sigma_1=\max_{\|x\|_2=1}\|Ax\|_2=\|A\|_2.
$$

Here the [operator norm](operator-norm.md) uses [Euclidean norm](euclidean-norm.md): no [unit vector](unit-vector.md) stretches more than fivefold. Zero [singular values](singular-value.md) identify lost directions; the number of positive [singular values](singular-value.md) equals the [matrix rank](matrix-rank.md). This summarizes both amplification and information loss with nonnegative numbers.[Verma, slides 7–8: singular values and maximum stretching](https://math.mit.edu/~gs/linearalgebra/ila5/SVD_Slides.pdf)

Small positive [singular values](singular-value.md) also explain sensitivity in an [inverse problem](inverse-problem-split.md). For a square [invertible matrix](invertible-matrix.md), the [matrix inverse](matrix-inverse.md) sends $u_j$ to $v_j/\sigma_j$: a weak forward response becomes strong inverse amplification. The [condition number](condition-number.md) for [Euclidean norm](euclidean-norm.md) is $\sigma_1/\sigma_n$, equal to $5$ in our example. To see a larger effect, keep the same [right singular vectors](right-singular-vector.md) but change the second [singular value](singular-value.md) to $\varepsilon=0.01$:

$$
A_\varepsilon=\begin{pmatrix}3&4\\-4\varepsilon/5&3\varepsilon/5\end{pmatrix},\qquad
\delta b=0.001u_2,\qquad
\delta x=A_\varepsilon^{-1}\delta b=0.1v_2=(-0.08,0.06)^T.
$$

The output perturbation has [Euclidean norm](euclidean-norm.md) $0.001$, but the recovered input changes by $0.1$. Its hundredfold amplification follows from the direction of the perturbation, not just its size. The [condition number](condition-number.md) is now $500$; it measures the disparity between the strongest and weakest responses.[Marschner, Condition numbers, §2: inverse amplification and singular values](https://www.cs.cornell.edu/courses/cs322/2007sp/notes/condition.pdf)

**Table of contents**

- [Right singular vector](right-singular-vector.md)
- [Left singular vector](left-singular-vector.md)

## ↑ Ancestors (6)

1. [Singular value decomposition](singular-value-decomposition.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (81)

- [Absolute value of an operator](absolute-value-of-an-operator.md)
- [Autonne-Takagi factorization](autonne-takagi-factorization.md)
- [Biadjacency matrix](biadjacency-matrix.md)
- [Box norm singular-value identity](box-norm-singular-value-identity.md)
- [Chiral-superfield fermion mass matrix](chiral-superfield-fermion-mass-matrix.md)
- [Directed subspace angle](directed-subspace-angle.md)
- [Eckart-Young-Mirsky theorem](eckart-young-mirsky-theorem.md)
- [Fitted values](fitted-values.md)
- [Gaussian posterior in the zero-noise limit](gaussian-posterior-in-the-zero-noise-limit.md)
- [Generalized singular vector](generalized-singular-vector.md)
- [Ill-posed inverse problem](ill-posed-inverse-problem.md)
- [Landweber full inverse filter](landweber-full-inverse-filter.md)
- [Left singular vector](left-singular-vector.md)
- [Low-rank approximation](low-rank-approximation.md)
- [Matrix 2-norm](matrix-2-norm.md)
- [Matrix Fourier block](matrix-fourier-block.md)
- [Matrix norm](matrix-norm.md)
- [Maximal dilatation](maximal-dilatation.md)
- [Moore-Penrose inverse](moore-penrose-inverse.md)
- [Normalized adjacency operator of a bipartite graph](normalized-adjacency-operator-of-a-bipartite-graph.md)
- [Overdetermined least-squares example](overdetermined-least-squares-example.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-53/3/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-79/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-80/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-9/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-1/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-48/3/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-70/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-78/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-31/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-36/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-72/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-72/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-48/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-76/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-76/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-76/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111/4/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-324/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-326/3/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-1/6b/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-132/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326/1/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326/2/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326/2/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-331/4/a/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-331/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-335/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-331/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-225/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-225/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-324/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-331/3/iii/b/solution.md)
- [Principal stretch](principal-stretch.md)
- [Quasirandom bipartite graph](quasirandom-bipartite-graph.md)
- [Rank-one update singularity criterion](rank-one-update-singularity-criterion.md)
- [Ridge regression](ridge-regression.md)
- [Right singular vector](right-singular-vector.md)
- [Singular matrix](singular-matrix.md)
- [Singular value](singular-value.md)
- [Singular value decomposition](singular-value-decomposition.md)
- [Small singular values in the Moore-Penrose inverse](small-singular-values-in-the-moore-penrose-inverse.md)
- [Source condition for quadratic regularization](source-condition-for-quadratic-regularization.md)
- [Spectral inverse theorem for the matrix-valued U2 quantity](spectral-inverse-theorem-for-the-matrix-valued-u2-quantity.md)
- [Tikhonov regularization](tikhonov-regularization.md)
- [Trace norm](trace-norm.md)
- [Unitary skew-diagonalization of an antisymmetric matrix](unitary-skew-diagonalization-of-an-antisymmetric-matrix.md)
