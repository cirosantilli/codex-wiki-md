<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write the surplus process in the [classical risk model](../../../../../classical-risk-model.md) as $U_t=u+ct-\sum_{j=1}^{N_t}X_j$, with positive independent claims. Condition on the first claim time, which has [exponential distribution](../../../../../exponential-distribution.md) of rate $\lambda$. If that claim occurs at $t$, the available capital is $u+ct$ and survival requires its size not to exceed that capital. The independent future process then gives

$$
\phi(u)=\int_0^\infty\lambda e^{-\lambda t}\int_0^{u+ct}\phi(u+ct-x)f(x)\,dx\,dt.
$$

Put $A(v)=\int_0^v\phi(v-x)f(x)\,dx$ and change variables $v=u+ct$. We obtain

$$
\phi(u)=\frac\lambda c e^{\lambda u/c}\int_u^\infty e^{-\lambda v/c}A(v)\,dv.
$$

The convolution of bounded $\phi$ with the integrable density is continuous; differentiation of this expression is therefore justified. It proves the survival version of the [ruin integro-differential equation](../../../../../ruin-integro-differential-equation.md):

$$
\boxed{\phi'(u)=\frac\lambda c\phi(u)-\frac\lambda c\int_0^u\phi(u-x)f(x)\,dx.}
$$

The density is a [hyperexponential distribution](../../../../../hyperexponential-distribution.md) with mixture weights $3/4,1/4$ and exponential rates $4,2$. Its total integral is one and its mean is

$$
\mu_X=3\int_0^\infty xe^{-4x}\,dx+\frac12\int_0^\infty xe^{-2x}\,dx
=\frac3{16}+\frac18=\frac5{16}.
$$

The [relative safety loading](../../../../../relative-safety-loading.md) means $c=(1+\rho)\lambda\mu_X$. Substitution of $\rho=3/5$ gives $c=\lambda/2$ and $\lambda/c=2$.

Set $A_a(u)=\int_0^u\phi(u-x)e^{-ax}\,dx$. Differentiating in its equivalent form $\int_0^u\phi(v)e^{-a(u-v)}\,dv$ gives $A_a'=\phi-aA_a$. The survival equation becomes

$$
\phi'=2\phi-6A_4-A_2.
$$

Apply the constant-coefficient operator $(D+4)(D+2)$, where $D=d/du$. Since $(D+4)A_4=\phi$ and $(D+2)A_2=\phi$,

$$
(D+4)(D+2)\phi'=2(D+4)(D+2)\phi-6(D+2)\phi-(D+4)\phi.
$$

Expanding and cancelling yields **$\boxed{\phi'''+4\phi''+3\phi'=0}$**. Thus $\phi(u)=A+Be^{-u}+Ce^{-3u}$.

Positive loading also fixes the limiting boundary value $\phi(u)\to1$. Indeed the aggregate-claims process minus premium income tends to minus infinity almost surely by the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md). Its supremum over all time is consequently finite almost surely, since paths have finitely many jumps on bounded intervals. The probability that this supremum exceeds $u$ tends to zero. Hence $A=1$. At zero, the given value is $\phi(0)=3/8$, and the integral equation supplies the extra condition $\phi'(0)=2\phi(0)=3/4$. Therefore

$$
B+C=-\frac58,\qquad -B-3C=\frac34,
$$

so $B=-9/16$ and $C=-1/16$. **The nonruin probability is**

$$
\boxed{\phi(u)=1-\frac9{16}e^{-u}-\frac1{16}e^{-3u}.}
$$

This is the [two-exponential-mixture survival probability](../../../../../two-exponential-mixture-survival-probability.md). It increases from $3/8$ to $1$ and satisfies the original integral equation, not just the differentiated equation; the zero-capital derivative condition prevents introducing extraneous solutions.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 27](../../paper-27-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
