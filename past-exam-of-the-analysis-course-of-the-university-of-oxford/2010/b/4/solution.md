<h1 id="b/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [Baire category theorem](../../../../baire-category-theorem.md) states that a nonempty complete [metric space](../../../../metric-space.md) cannot be a countable union of closed [nowhere dense sets](../../../../nowhere-dense-set.md). The [Uniform boundedness principle](../../../../uniform-boundedness-principle.md) says that if $V$ is a [Banach space](../../../../banach-space-split.md), $W$ a [normed vector space](../../../../normed-vector-space-split.md), and $\mathcal T\subseteq B(V,W)$ is [pointwise](../../../../pointwise-convergence.md) bounded, meaning $\sup_{T\in\mathcal T}\|Tx\|<\infty$ for every $x\in V$, then $\sup_{T\in\mathcal T}\|T\|<\infty$.

To prove it, let $E_n=\{x:\sup_{T\in\mathcal T}\|Tx\|\leq n\}$. Each set is closed by [continuity](../../../../continuous-function.md) of the individual operators, and their union is $V$. The [Baire category theorem](../../../../baire-category-theorem.md) gives a ball $B(x_0,r)$ inside some $E_N$. For $\|h\|<r$, both $x_0+h$ and $x_0$ are in $E_N$, so $\|Th\|\leq\|T(x_0+h)\|+\|Tx_0\|\leq2N$ for every $T$. Scaling gives $\|T\|\leq2N/r$ uniformly. The zero-space and empty-family cases are immediate.

For the first family on a [Hilbert space](../../../../hilbert-space-split.md), fix $x$. The functionals $y\mapsto\langle y,Tx\rangle$ have [operator norm](../../../../operator-norm.md) $\|Tx\|$ by the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) and equality on the direction of $Tx$. Their values are [pointwise](../../../../pointwise-convergence.md) bounded by the hypothesis, after taking complex conjugates if necessary. Apply the [Uniform boundedness principle](../../../../uniform-boundedness-principle.md) to obtain $\sup_{T\in\mathcal E}\|Tx\|<\infty$. Apply it a second time to the operator family itself to conclude **$\sup_{T\in\mathcal E}\|T\|<\infty$**.

For the diagonal hypothesis, the answer depends on the scalar [field](../../../../field.md). Over $\mathbb C$, let $q_T(x)=\langle Tx,x\rangle$, using the convention that the [inner product](../../../../inner-product-split.md) is linear in its first variable. The complex [polarization identity](../../../../polarization-identity.md) gives

$$
4\langle Tx,y\rangle=q_T(x+y)-q_T(x-y)+i q_T(x+iy)-i q_T(x-iy).
$$

The assumed bounds at these four fixed vectors make every matrix coefficient uniformly bounded, so the preceding argument applies. Thus **the complex-space answer is yes**, even without assuming self-adjointness.

Over $\mathbb R$, take $X=\mathbb R^2$ and

$$
J=\begin{pmatrix}0&-1\\1&0\end{pmatrix},\qquad\mathcal F=\{nJ:n\geq1\}.
$$

Every diagonal value $\langle nJx,x\rangle$ is zero, whereas $\|nJ\|=n$. Thus **the real-space answer is no in general**. Real diagonal values do not detect the skew-symmetric part of an operator. This is [diagonal boundedness of operator families over real and complex Hilbert spaces](../../../../diagonal-boundedness-of-operator-families-over-real-and-complex-hilbert-spaces.md).

## ↑ Ancestors (12)

1. [4](../4.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
