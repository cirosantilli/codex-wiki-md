<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

At a target $x$, the degree-$p$ [local polynomial regression](../../../../../local-polynomial-regression.md) estimate minimizes

$$
\sum_{i=1}^nK\left(\frac{x_i-x}{h}\right)
\left\{Y_i-\sum_{j=0}^pb_j(x_i-x)^j\right\}^2,
$$

and $\widehat m_n(x;p,h,K)=\widehat b_0$. Let $R_x$ have row  
$(1,x_i-x,\ldots,(x_i-x)^p)$ and let $W_x$ be diagonal with the kernel weights. Assume the [local polynomial Gram matrix](../../../../../local-polynomial-gram-matrix.md) $R_x^TW_xR_x$ is positive definite. The weighted normal equations give

$$
\widehat m_n(x;p,h,K)
=e_1^T(R_x^TW_xR_x)^{-1}R_x^TW_xY,
$$

so it is a [linear estimator in nonparametric regression](../../../../../linear-estimator-in-nonparametric-regression.md).

Define

$$
s_r(x)=\frac1{nh}\sum_{i=1}^n(x_i-x)^r
K\left(\frac{x_i-x}{h}\right).
$$

Inverting the two-by-two Gram matrix for $p=1$ yields

$$
\widehat m_n(x;1,h,K)
=\frac1{nh}\sum_{i=1}^n
\frac{s_2(x)-s_1(x)(x_i-x)}
{s_2(x)s_0(x)-s_1(x)^2}
K\left(\frac{x_i-x}{h}\right)Y_i.
$$

Now put $M=\min\{n,\lfloor nh\rfloor\}$. At $x=0$ and for the uniform kernel,

$$
s_r=\frac1{2nh\,n^r}\sum_{i=1}^Mi^r.
$$

For the usual bandwidth range $0<h\leq1$, $M=\lfloor nh\rfloor$. The elementary power-sum formulas and $|M-nh|\leq1$ show, for $r=0,1,2,3$, that

$$
\left|s_r-\frac{h^r}{2(r+1)}\right|
\leq C_r\frac{h^r}{nh}
$$

The limiting moment determinant is

$$
\frac12\frac{h^2}{6}-\left(\frac h4\right)^2
=\frac{h^2}{48}.
$$

For $nh\geq32$, the displayed errors can consume at most a fixed fraction of this value, so

$$
s_2s_0-s_1^2\geq ch^2
$$

for a universal $c>0$ and $0<h\leq1$.

As printed, the claim “for all $h>0$” cannot hold for this design: if $h>1$, all $n$ points receive weight $1/2$, each $s_r=O(h^{-1})$, and the determinant is $O(h^{-2})$, not bounded below by a positive multiple of $h^2$. The standard bandwidth restriction $h\leq1$ is therefore necessary for that intermediate assertion. The final bias bound remains harmless for $h>1$, since $h^2\geq1$ and the finite design response means are uniformly bounded.

The [polynomial reproduction property of local polynomial regression](../../../../../polynomial-reproduction-property-of-local-polynomial-regression.md) makes the local-linear weights reproduce both $1$ and $u$. Write

$$
e^{x_i}=1+x_i+R_i,\qquad |R_i|\leq Cx_i^2
$$

for $0\leq x_i\leq\min(h,1)$. The reproduced terms have zero bias. Using $s_r=O(h^r)$, the numerator contributed by the remainders is bounded by

$$
C\{s_2s_2+s_1s_3\}=O(h^4).
$$

Division by the determinant lower bound gives

$$
\left|\operatorname{Bias}\widehat m_n(0;1,h,K)\right|\leq Ch^2.
$$

The degree-zero [Nadaraya–Watson estimator](../../../../../nadaraya-watson-estimator.md) reproduces constants but not linear functions. The term $x_i$ therefore remains, and its boundary bias is bounded by $Ch$; this first-order boundary bias is the improvement that local linear fitting removes.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
