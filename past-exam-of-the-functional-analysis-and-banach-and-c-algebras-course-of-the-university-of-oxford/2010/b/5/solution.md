<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a [self-adjoint C-star element](../../../../hermitian-element-of-a-c-star-algebra.md) $a$, the following are three equivalent characterizations of a [Positive element of a C-star algebra](../../../../positive-element-of-a-c-star-algebra.md):

$$
\boxed{\begin{aligned}
&\sigma(a)\subseteq[0,\infty);\\
&\|a-\|a\|1_A\|\leq\|a\|;\\
&\text{there is }t>0\text{ with }\|a-t1_A\|\leq t.
\end{aligned}}
$$

If $a=b^2$ with $b=b^*$, the [spectral mapping theorem](../../../../spectral-mapping-theorem.md) gives nonnegative spectrum. Conversely, the [continuous functional calculus](../../../../continuous-functional-calculus.md) applied to $\sqrt{\lambda}$ on $\sigma(a)$ gives a [self-adjoint C-star element](../../../../hermitian-element-of-a-c-star-algebra.md) $b$ with $b^2=a$. For real $\sigma(a)$,

$$
\|a-t1_A\|=\max_{\lambda\in\sigma(a)}|\lambda-t|.
$$

Thus the third condition means $\sigma(a)\subseteq[0,2t]$, while the first implies the second by taking the interval $[0,\|a\|]$. The second implies the third with $t=\|a\|$ if $a\ne0$; if $a=0$, any $t>0$ works. This proves every equivalence.

The [positive cone of a C-star algebra](../../../../positive-cone-of-a-c-star-algebra.md) contains zero and is closed under multiplication by nonnegative real scalars. To verify addition without assuming that positive elements commute, put $r=\|a\|$, $s=\|b\|$ for $a,b\geq0$. Then

$$
\|(a+b)-(r+s)1_A\|\leq\|a-r1_A\|+\|b-s1_A\|\leq r+s.
$$

If $r+s>0$, the third characterization makes $a+b$ positive; otherwise both are zero. Hence it is a [convex cone](../../../../convex-cone.md). If $a$ and $-a$ are positive, $\sigma(a)=\{0\}$ and $a=0$ by the [self-adjoint](../../../../self-adjoint-operator.md) spectral [norm](../../../../norm.md) formula; therefore the cone is pointed and defines a [partial order](../../../../partially-ordered-set.md) on $A_{\mathrm{sa}}$ by $h\leq k$ if $k-h\in A_+$. It is generating because the [continuous functional calculus](../../../../continuous-functional-calculus.md) gives

$$
|h|=(h^2)^{1/2},\qquad h_\pm=\tfrac12(|h|\pm h)\geq0,\qquad h=h_+-h_-.
$$

For $a\geq0$, the [spectral mapping theorem](../../../../spectral-mapping-theorem.md) yields

$$
\boxed{\|a\|\leq1\iff\sigma(a)\subseteq[0,1]\iff1_A-a\geq0\iff0\leq a\leq1_A.}
$$

Finally, let $a\in M_2(\mathbb C)$ be [Hermitian](../../../../hermitian-operator.md), and write $\tau=\operatorname{tr}a$, $d=\det a$. Its two [eigenvalues](../../../../eigenvalue.md) are real. Both are nonnegative exactly when their sum $\tau$ and product $d$ are nonnegative. The corresponding sum and product for $I-a$ are $2-\tau$ and $1-\tau+d$. Therefore the necessary and sufficient conditions for a [positive contraction](../../../../positive-contraction.md) are

$$
\boxed{0\leq\tau\leq2,\qquad d\geq0,\qquad1-\tau+d\geq0.}
$$

Indeed, nonnegative sum and product force two real numbers to be nonnegative, including the zero-product cases. Applying this to $a$ and $I-a$ places both [eigenvalues](../../../../eigenvalue.md) in $[0,1]$.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../split.md)
5. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
