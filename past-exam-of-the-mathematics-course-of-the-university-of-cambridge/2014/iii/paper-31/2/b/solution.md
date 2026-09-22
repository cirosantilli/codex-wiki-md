<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the original [exponential distribution](../../../../../../exponential-distribution.md), cancel the nonzero root in

$$
\frac{1}{1-\mu R}-1=(1+\theta)\mu R
$$

to obtain

$$
\boxed{R_{\rm old}=\frac{\theta}{(1+\theta)\mu}.}
$$

It lies strictly below the transform pole $1/\mu$.

With the extra expenses, the insurer's payment per claim is $Y=X+A$, where $A$ has [exponential distribution](../../../../../../exponential-distribution.md) of [expected value](../../../../../../expected-value.md) $\mu/2$ and is independent of $X$. The [convolution of independent random variables](../../../../../../convolution-of-independent-random-variables.md) gives a [hypoexponential distribution](../../../../../../hypoexponential-distribution.md) with

$$
\mathbb EY=\frac32\mu,\qquad M_Y(r)=\frac{1}{(1-\mu r)(1-\mu r/2)},\quad r<1/\mu.
$$

Keeping the [relative safety loading](../../../../../../relative-safety-loading.md) fixed means using the new expected payment: the premium rate becomes $c_{\rm new}=\lambda(1+\theta)(3\mu/2)$. It does not mean keeping the old premium rate fixed. The [adjustment coefficient with independent claim expenses](../../../../../../adjustment-coefficient-with-independent-claim-expenses.md) therefore solves

$$
\frac{1}{(1-\mu R)(1-\mu R/2)}-1=(1+\theta)\frac32\mu R.
$$

Set $t=\mu R$, cancel $t>0$, and simplify:

$$
3(1+\theta)t^2-(7+9\theta)t+6\theta=0.
$$

The quadratic is positive at $t=0$ and equals $-4$ at $t=1$. Its leading coefficient is positive, so the smaller root is in $(0,1)$ and the larger root exceeds $1$. Only the smaller root lies in the finite [moment-generating function](../../../../../../moment-generating-function.md) domain. Hence

$$
\boxed{R_{\rm new}=\frac{7+9\theta-\sqrt{9\theta^2+54\theta+49}}
{6(1+\theta)\mu}.}
$$

For $\theta=1$,

$$
\boxed{R_{\rm old}=\frac{1}{2\mu},\qquad
R_{\rm new}=\frac{4-\sqrt7}{3\mu}\approx\frac{0.451416}{\mu},\qquad
\frac{R_{\rm new}}{R_{\rm old}}=\frac{2(4-\sqrt7)}{3}\approx0.902832.}
$$

Thus **the new adjustment coefficient is about $9.72\%$ smaller**, even though the premium rate has been increased to retain the same [relative safety loading](../../../../../../relative-safety-loading.md). The [Lundberg inequality](../../../../../../lundberg-inequality.md) consequently has a slower exponential decay rate as a function of capital.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
