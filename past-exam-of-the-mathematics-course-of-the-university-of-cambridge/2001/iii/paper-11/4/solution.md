<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the independent [product measure](../../../../../product-measure.md) on the finite coordinate spaces. For $A\ne\varnothing$, let $V_A(x)$ be the [convex hull](../../../../../convex-hull.md) of its mismatch vectors $(\mathbf1_{x_i\ne y_i})_{i=1}^n$, $y\in A$. The distance in the question equals

$$
d_T(x,A)=\min_{v\in V_A(x)}\|v\|_2.
$$

To verify this, let $v_*$ be the nearest point. Any unit vector $\alpha$ satisfies $\min_{v\in V_A}\alpha\cdot v\le\alpha\cdot v_*\le\|v_*\|_2$. Conversely the projection property $v_*\cdot(v-v_*)\ge0$ gives equality for $\alpha=v_*/\|v_*\|_2$ when $v_*\ne0$. If $v_*=0$, nonnegative weights give supremum zero. Linear functionals have the same minimum on the hull as on its original vectors, so this is exactly the quantified definition of the [Talagrand convex distance](../../../../../talagrand-convex-distance.md).

We prove the stronger [section induction for the Talagrand exponential moment](../../../../../section-induction-for-the-talagrand-exponential-moment.md),

$$
\boxed{\mathbb E\exp(d_T(X,A)^2/4)\le\frac1{\Pr(A)}\qquad(\Pr(A)>0).}
$$

Zero-probability atoms may be discarded, replacing $A$ by its supported part: this preserves its [probability](../../../../../probability.md) and can only increase its distance. Thus assume all coordinate atoms have positive mass. The induction starts with zero coordinates, when a positive-probability event is the singleton space and its distance is zero.

Split the last coordinate into values $j$, with [probabilities](../../../../../probability.md) $q_j$, and write $A_j$ for the corresponding section in the first $n-1$ coordinates. Put $a_j=\Pr(A_j)$, choose a largest section $A_s$ of [probability](../../../../../probability.md) $a>0$, and set $r_j=a_j/a\in[0,1]$. For a point $(x',j)$, mix nearest mismatch vectors from $A_j$ and $A_s$ with weights $\lambda,1-\lambda$. Their final coordinates are zero and, if $j\ne s$, one. Convexity of the squared norm gives

$$
d_T((x',j),A)^2
\le\lambda d_T(x',A_j)^2+(1-\lambda)d_T(x',A_s)^2+(1-\lambda)^2.
$$

For an empty $A_j$, use $\lambda=0$ directly. If $j=s$, the final-coordinate term is an unnecessary nonnegative allowance, so the bound still holds.

Exponentiate, integrate in $x'$, and use [Hölder's inequality](../../../../../holder-s-inequality.md) and the induction hypothesis. For $r_j>0$ this gives

$$
\mathbb E_{x'}e^{d_T((x',j),A)^2/4}
\le\frac1a\inf_{0\le\lambda\le1}r_j^{-\lambda}e^{(1-\lambda)^2/4}
\le\frac{2-r_j}{a}.
$$

We supply the [scalar estimate for Talagrand product induction](../../../../../scalar-estimate-for-talagrand-product-induction.md) used in the last step. Set $L=-\log r$. For $0\le L\le1/2$, choose $1-\lambda=2L$, making the expression $e^{L-L^2}$. The function

$$
h(L)=\log(2-e^{-L})-L+L^2
$$

has $h(0)=h'(0)=0$ and

$$
h''(L)=2-\frac{2e^L}{(2e^L-1)^2}\ge0\qquad(L\ge0).
$$

Thus $e^{L-L^2}\le2-e^{-L}$. For $L\ge1/2$, choose $\lambda=0$, giving $e^{1/4}$; the already proved boundary case and monotonicity of $2-e^{-L}$ give the same bound. For $r=0$, the direct empty-section bound is $e^{1/4}/a\le2/a$.

Now average over $j$. With $m=\sum_jq_jr_j=\Pr(A)/a\in(0,1]$, the exponential integral is at most $(2-m)/a$. Since $m(2-m)\le1$, this is at most $1/(am)=1/\Pr(A)$, closing the induction.

Finally apply the [Markov inequality](../../../../../markov-inequality.md) to the nonnegative exponential. For the distance-tail event $\overline A_t$,

$$
\boxed{\Pr(A)\Pr(\overline A_t)\le e^{-t^2/4}\qquad(t\ge0).}
$$

This proves [Talagrand's convex distance inequality](../../../../../talagrand-s-convex-distance-inequality.md) for the finite product. If $\Pr(A)=0$, the required probability-product inequality is immediate, including the empty-event case with distance defined as infinity; no finite exponential-moment assertion is needed there.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
