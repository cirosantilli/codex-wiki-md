<h1 id="13e/solution">Solution</h1>

↑ **Parent:** [13E](../13e.md)

Write $L(f)=\sup_{x\ne y}|f(x)-f(y)|/d(x,y)$ and $B(f)=\sup_z|f(z)|$. The quantity in the question is the [bounded Lipschitz norm](../../../../../bounded-lipschitz-norm.md) $\|f\|_{\rm BL}=L(f)+B(f)$. Both terms are nonnegative and absolutely homogeneous, and each satisfies the [triangle inequality](../../../../../triangle-inequality.md). Therefore their sum does too; finite values are preserved by addition and scalar multiplication, making the domain a [vector space](../../../../../vector-space-split.md). If the sum is zero, $B(f)=0$ forces $f=0$. Thus it is a [norm](../../../../../norm.md).

For the sequence bounded by one, both $L(f_i)\leq1$ and $B(f_i)\leq1$. Given real $x$, choose a nearby rational $q$. Then

$$
|f_i(x)-f_j(x)|\leq2|x-q|+|f_i(q)-f_j(q)|.
$$

First make $|x-q|$ small, then use convergence at $q$ to make the last term small. The values at every real $x$ form a [Cauchy sequence](../../../../../cauchy-sequence.md), so $f_i$ converges pointwise to a real function $f$.

To preserve the sum bound rather than merely bound its two terms separately, use every fixed triple $x\ne y,z$:

$$
\frac{|f_i(x)-f_i(y)|}{|x-y|}+|f_i(z)|\leq1.
$$

Pass to the pointwise limit and take the independent suprema over $(x,y)$ and $z$. This gives $\boxed{\|f\|_{\rm BL}\leq1}$, the [pointwise closure of the bounded Lipschitz unit ball](../../../../../pointwise-closure-of-the-bounded-lipschitz-unit-ball.md).

To obtain [diagonal compactness for bounded Lipschitz functions](../../../../../diagonal-compactness-for-bounded-lipschitz-functions.md), enumerate the rationals for an arbitrary sequence in this unit ball. Values at the first rational lie in $[-1,1]$, so the [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md) supplies a convergent subsequence there. Repeatedly extract nested subsequences for successive rationals. The [diagonal subsequence argument](../../../../../diagonal-subsequence-argument.md) gives one subsequence converging at every rational. Applying the preceding argument proves **there is a pointwise convergent subsequence with limit of bounded Lipschitz norm at most one**.

## ↑ Ancestors (10)

1. [13E](../13e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
