<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

With the centred data, no intercept is needed. Use the [Lasso](../../../../../lasso.md) normalization

$$
\boxed{\widehat\beta^L_\lambda\in\operatorname*{arg\,min}_{b\in\mathbb R^p}\left\{\frac1{2n}\|Y-Xb\|_2^2+\lambda\|b\|_1\right\}.}
$$

Write $r=Y-Xb$ and $c=X^{\mathsf T}r/n$. The [KKT conditions](../../../../../karush-kuhn-tucker-conditions.md) are

$$
\boxed{c_k=\lambda\operatorname{sign}(b_k)\text{ if }b_k\ne0,\qquad |c_k|\leq\lambda\text{ if }b_k=0.}
$$

Indeed, the [subdifferential of the L1 norm](../../../../../subdifferential-of-the-l1-norm.md) consists of vectors $z$ with $z_k=\operatorname{sign}(b_k)$ at nonzero coordinates and $z_k\in[-1,1]$ at zero coordinates. The [subgradient optimality condition](../../../../../subgradient-optimality-condition.md) is $0=-X^{\mathsf T}(Y-Xb)/n+\lambda z$. [convexity](../../../../../convex-function.md) makes these conditions sufficient as well as necessary. These are the [Karush-Kuhn-Tucker conditions for the Lasso](../../../../../karush-kuhn-tucker-conditions-for-the-lasso.md).

Here is a correlation-parameter version of [least angle regression](../../../../../least-angle-regression.md). Put $G=X^{\mathsf T}X/n$, a [Gram matrix](../../../../../gram-matrix.md), and initialize $\widehat\beta=0$, $A_1=\varnothing$, $\lambda_0=\infty$.

1. Compute $\lambda_1=\max_k|X_k^{\mathsf T}Y|/n$. For $\lambda\geq\lambda_1$, keep $\widehat\beta(\lambda)=0$. If $\lambda_1=0$, stop: all [regression residual](../../../../../regression-residual.md) correlations already vanish. Otherwise add the uniquely maximizing variable to obtain $A_2$.
1. At step $m\geq2$, put $t=\lambda_{m-1}$, $A=A_m$, $b^0=\widehat\beta(t)$, and $s_A=c_A(t)/t$. These active signs have entries in $\{-1,1\}$. Solve $G_{AA}d_A=s_A$, set $d_{A^c}=0$, and follow the segment$$
   \widehat\beta(\lambda)=b^0+(t-\lambda)d,\qquad0\leq\lambda\leq t.
   $$
1. For each inactive variable set $a_j=G_{jA}d_A$. Along the segment its correlation is $c_j(t)-h a_j$, where $h=t-\lambda$. Its candidate hitting distances are$$
   h_j^+=\frac{t-c_j(t)}{1-a_j},\qquad h_j^-=\frac{t+c_j(t)}{1+a_j}.
   $$

   Discard undefined or nonpositive candidates. Choose the smallest remaining distance below $t$, if one exists, and otherwise choose $h=t$. Set $\lambda_m=t-h$. If $\lambda_m>0$, add the unique variable achieving the hit to form $A_{m+1}$ and repeat; if $\lambda_m=0$, stop.

The two hitting formulas come from $c_j(t)-h a_j=\pm(t-h)$. This is [LAR hitting time](../../../../../entry-knot-in-least-angle-regression.md). Active variables are not dropped if a coefficient crosses zero: that is the distinction between this algorithm and the modified [Lasso](../../../../../lasso.md) path algorithm.

The active [Gram matrix](../../../../../gram-matrix.md) is an [invertible matrix](../../../../../invertible-matrix.md) under the assumed unique positive hits. Inductively, a candidate column in the span of the current active columns would have $c_j(\lambda)$ equal to a fixed linear combination of their correlations, hence proportional to $\lambda$ on the whole segment. Its ratio $|c_j(\lambda)|/\lambda$ could not first reach one at a positive interior knot. Thus every uniquely entering column adds a new independent direction. This also allows more predictors than observations; the algorithm stops before a dependent direction needs to be added at zero correlation.

We now prove the requested invariant. At the first positive knot the newly active correlation has magnitude $\lambda_1$. At a later knot the old active correlations have that knot's magnitude by induction, and the entering correlation has the same magnitude by the hitting rule. Throughout the next segment,

$$
c_A(\lambda)=c_A(t)-(t-\lambda)G_{AA}d_A=t s_A-(t-\lambda)s_A=\lambda s_A.
$$

The first-hitting rule also ensures $|c_j(\lambda)|\leq\lambda$ for every inactive $j$. If no positive hit remains, this inequality continues to zero, where all correlations vanish. Consequently, on every printed closed segment,

$$
\boxed{\frac1n|X_k^{\mathsf T}(Y-X\widehat\beta(\lambda))|=\lambda\quad(k\in A_m).}
$$

This is the [LAR active correlation invariant](../../../../../lar-active-correlation-invariant.md).

If active nonzero coefficients have the same signs as their residual correlations, the active equalities are precisely the nonzero-coordinate [Lasso](../../../../../lasso.md) [KKT conditions](../../../../../karush-kuhn-tucker-conditions.md). An active coefficient which is zero also satisfies the zero-coordinate [KKT conditions](../../../../../karush-kuhn-tucker-conditions.md), because its correlation is within $[-\lambda,\lambda]$. Inactive coefficients are zero and satisfy those same inequalities by construction. Thus every point of the [least angle regression](../../../../../least-angle-regression.md) path is a [Lasso](../../../../../lasso.md) minimizer for $\lambda>0$. Under the stated uniqueness assumption,

$$
\boxed{\widehat\beta(\lambda)=\widehat\beta^L_\lambda\qquad(\lambda>0).}
$$

This proves the desired implication, in fact under the weaker [sign compatibility of LAR and Lasso](../../../../../sign-compatibility-of-lar-and-lasso.md) condition requiring agreement only at nonzero coefficients.

There is an endpoint convention in the printed sufficient condition. With the standard $\operatorname{sign}(0)=0$, a newly entering coefficient is zero at a positive knot although its correlation is $\pm\lambda$; the displayed sign equality therefore cannot literally hold there. At the final zero knot the correlation signs are zero as well. Interpret sign compatibility on positive open segments, or in the nonzero-coefficient/subgradient sense just proved. The [KKT conditions](../../../../../karush-kuhn-tucker-conditions.md) already handle zero coefficients at knots, and no equality of solution paths at $\lambda=0$ is needed for the requested conclusion.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
