<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use a nonzero complex unital [Banach algebra](../../../../../banach-algebra-split.md) $B$ with submultiplicative [norm](../../../../../norm.md), and write its [unit](../../../../../unit-in-a-ring.md) as $e$. The complex [scalar field](../../../../../scalar-field.md) is the usual convention in this spectral statement; for a real algebra one uses its complexification. We derive the needed analytic facts from norm-convergent series and scalar complex analysis.

If $\|a\|<1$, [completeness](../../../../../completeness.md) makes the [Neumann series](../../../../../neumann-series.md) $\sum_{j=0}^\infty a^j$ converge. Multiplying its finite partial sums by $e-a$ gives $e-a^{m+1}$, which tends to $e$. Hence its sum is the inverse of $e-a$. If $b$ is invertible, then $b+h=b(e+b^{-1}h)$ is invertible whenever $\|b^{-1}h\|<1$. This proves that the invertible elements form an [open set](../../../../../open-set.md) and that inversion is locally norm-continuous.

Define the [Banach algebra spectrum](../../../../../spectrum-of-an-element.md) and the [resolvent of an element](../../../../../resolvent-of-an-element.md) by

$$
\sigma(x)=\{\lambda\in\mathbb C:\lambda e-x\text{ is not invertible}\},
\qquad R(\lambda)=(\lambda e-x)^{-1}\quad(\lambda\notin\sigma(x)).
$$

For $|\lambda|>\|x\|$, the [Neumann series](../../../../../neumann-series.md) gives

$$
\boxed{R(\lambda)=\sum_{j=0}^\infty\frac{x^j}{\lambda^{j+1}},\qquad x^0=e.}
$$

Thus $\sigma(x)$ is bounded by $\|x\|$ and is [closed](../../../../../closed-set.md), because invertibility is open. Also $R(\lambda)\to0$ in [norm](../../../../../norm.md) at infinity; for example its [norm](../../../../../norm.md) is at most $\|e\|/(|\lambda|-\|x\|)$, since $\|e\|\geq1$ in a nonzero submultiplicative unital algebra. The standard normalization $\|e\|=1$ is not needed.

For points where the [Banach algebra resolvent](../../../../../resolvent-of-an-element.md) exists $\lambda,\mu$, multiply out the inverses to get the [resolvent identity](../../../../../resolvent-identity.md)

$$
\boxed{R(\lambda)-R(\mu)=(\mu-\lambda)R(\lambda)R(\mu).}
$$

For $\lambda_0$ outside the [Banach algebra spectrum](../../../../../spectrum-of-an-element.md), put $R_0=R(\lambda_0)$. Locally,

$$
R(\lambda_0+h)=R_0(e+hR_0)^{-1}
=\sum_{j=0}^\infty(-h)^jR_0^{j+1},\qquad |h|\|R_0\|<1.
$$

This series and its differentiated series converge uniformly on every smaller disk. It therefore proves $R$ is a [Banach-space-valued holomorphic function](../../../../../banach-space-valued-holomorphic-function.md), establishing complex differentiability in the Banach-space [norm](../../../../../norm.md) and gives $R'=-R^2$, without assuming a Banach-algebra-valued analytic theorem. In particular every [continuous](../../../../../continuous-function.md) complex [linear functional](../../../../../linear-functional.md) $\phi$ makes $\phi(R(\lambda))$ a scalar [holomorphic function](../../../../../holomorphic-function.md).

The [Banach algebra spectrum](../../../../../spectrum-of-an-element.md) is nonempty. Otherwise $R$ would be defined and analytic everywhere. Its local [norm](../../../../../norm.md) continuity and decay at infinity make it globally bounded. For every [continuous linear functional](../../../../../continuous-linear-functional.md) $\phi$, the scalar [entire function](../../../../../entire-function.md) $\phi(R(\lambda))$ is bounded and tends to zero at infinity, so it is identically zero: the scalar [Cauchy estimate](../../../../../cauchy-estimate.md) for its [derivative](../../../../../derivative.md) on circles of radius $r$ is $M/r$, which tends to zero, and the limiting value then fixes its constant as zero. Such functionals separate points by the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md). Explicitly a bounded real functional can be extended from the real span of any nonzero element using its [norm](../../../../../norm.md), and complexifying it by $\phi(v)=\ell(v)-i\ell(iv)$ gives a bounded complex [linear functional](../../../../../linear-functional.md) nonzero on that element. Therefore $R$ itself would be zero, contradicting $(\lambda e-x)R=e$. We have proved **the [Banach algebra spectrum](../../../../../spectrum-of-an-element.md) is a nonempty compact subset of the [complex plane](../../../../../complex-plane.md)**.

We next establish the [spectral radius formula](../../../../../spectral-radius-formula.md). The power norms are submultiplicative. If some $x^m=0$, their root norms are eventually zero. Otherwise, for any fixed $m$, write $n=qm+r$ with $0\leq r<m$ to obtain

$$
\|x^n\|\leq\|x^m\|^q\max_{0\leq r<m}\|x^r\|.
$$

Taking roots gives $\limsup_n\|x^n\|^{1/n}\leq\|x^m\|^{1/m}$. Taking the [infimum](../../../../../infimum.md) in $m$, and using that every root [norm](../../../../../norm.md) is at least that [infimum](../../../../../infimum.md), proves existence of

$$
\rho_0=\lim_{n\to\infty}\|x^n\|^{1/n}
=\inf_{m\geq1}\|x^m\|^{1/m}.
$$

For $|\lambda|>\rho_0$, the [root test](../../../../../root-test.md) makes $\sum x^j/\lambda^{j+1}$ converge, even when $|\lambda|\leq\|x\|$. The same telescoping [multiplication](../../../../../multiplication.md) proves it is a two-sided inverse. Hence

$$
r_\sigma:=\max_{\lambda\in\sigma(x)}|\lambda|\leq\rho_0.
$$

For the reverse bound fix $R>r_\sigma$. If $R_1>\max(R,\|x\|)$, integrate the uniformly convergent exterior series term by term on $|\lambda|=R_1$, obtaining

$$
x^n=\frac1{2\pi i}\int_{|\lambda|=R_1}\lambda^nR(\lambda)\,d\lambda.
$$

The same integral equals the one on $|\lambda|=R$: applying an arbitrary [continuous linear functional](../../../../../continuous-linear-functional.md) reduces [contour deformation](../../../../../contour-deformation.md) through the [Banach algebra spectrum](../../../../../spectrum-of-an-element.md)-free annulus to the scalar [Cauchy theorem](../../../../../cauchy-s-integral-theorem.md), and separation of points restores equality in $B$. This proves the [resolvent Cauchy coefficient formula](../../../../../resolvent-cauchy-coefficient-formula.md) rather than assuming vector-valued analytic calculus. Using the [norm](../../../../../norm.md) bound for the allowed vector integral gives

$$
\|x^n\|\leq R^{n+1}\max_{|\lambda|=R}\|R(\lambda)\|.
$$

Taking $n$th roots yields $\rho_0\leq R$, and letting $R\downarrow r_\sigma$ finishes the proof:

$$
\boxed{\rho(x)=\lim_{n\to\infty}\|x^n\|^{1/n}
=\max_{\lambda\in\sigma(x)}|\lambda|
=\sup\{|\lambda|:\lambda e-x\text{ is not invertible}\}.}
$$

For the first example take the [commutative algebra](../../../../../commutative-algebra-split.md) of [dual numbers](../../../../../dual-number.md) $B=\mathbb C[\varepsilon]/(\varepsilon^2)$ with [norm](../../../../../norm.md) $\|a+b\varepsilon\|=|a|+|b|$. [Completeness](../../../../../completeness.md) follows from finite dimension, and the product estimate makes the [norm](../../../../../norm.md) submultiplicative. For $x=\varepsilon$, $x\ne0$ but $x^2=0$, so $\rho(x)=0$. Directly, $\lambda e-\varepsilon$ has inverse $\lambda^{-1}e+\lambda^{-2}\varepsilon$ for $\lambda\ne0$, and its [Banach algebra spectrum](../../../../../spectrum-of-an-element.md) is $\{0\}$. For the second example take $B=\mathbb C$ with its absolute-value [norm](../../../../../norm.md) and $x=1$. Its [Banach algebra spectrum](../../../../../spectrum-of-an-element.md) is $\{1\}$, giving **$\rho(x)=\|x\|=1$**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
