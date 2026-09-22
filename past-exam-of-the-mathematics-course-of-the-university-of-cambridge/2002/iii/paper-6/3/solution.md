<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Work in a nonzero complex unital [Banach algebra](../../../../../banach-algebra-split.md) $B$, with identity $1$. Write $R(x)=\{\lambda\in\mathbb C:\lambda1-x\text{ is invertible}\}$ for the resolvent set, $\sigma(x)=\mathbb C\setminus R(x)$ for the [spectrum of an element](../../../../../spectrum-of-an-element.md), and $Q(\lambda)=(\lambda1-x)^{-1}$ for its [Banach algebra resolvent](../../../../../resolvent-of-an-element.md). Distinguishing the set from the inverse-valued function avoids a notational ambiguity.

**The printed formula omits an essential modulus.** Complex spectral values cannot be ordered to take the indicated supremum. Even for $x=-1$ in $B=\mathbb C$, the spectrum is $\{-1\}$ while the [spectral radius](../../../../../spectral-radius.md) is one. The correctly interpreted assertion, proved below, is

$$
\boxed{\rho(x)=\lim_{n\to\infty}\|x^n\|^{1/n}=\max_{\lambda\notin R(x)}|\lambda|.}
$$

All required analytic facts about the [Banach algebra resolvent](../../../../../resolvent-of-an-element.md) will be derived from norm-convergent series and scalar complex analysis.

For $\|a\|<1$, the [Neumann series](../../../../../neumann-series.md) $\sum_{n\ge0}a^n$ converges in $B$ and is a two-sided inverse of $1-a$: multiplying its finite sums gives $1-a^{N+1}$ and passing to the limit gives $1$. Therefore for $|\lambda|>\|x\|$,

$$
Q(\lambda)=\sum_{n=0}^\infty\frac{x^n}{\lambda^{n+1}}.
$$

The series converges locally uniformly on that exterior region and tends to zero in norm as $|\lambda|\to\infty$. This statement does not require the optional normalization $\|1\|=1$; the zeroth term is $1/\lambda$, and the other terms have the usual geometric bound.

At any $\lambda_0\in R(x)$, factor $\lambda_01-x+h1=(\lambda_01-x)(1+hQ(\lambda_0))$. If $|h|\|Q(\lambda_0)\|<1$, the [Neumann series](../../../../../neumann-series.md) gives

$$
Q(\lambda_0+h)=\sum_{j=0}^\infty(-h)^jQ(\lambda_0)^{j+1}.
$$

Thus the resolvent set is open, $Q$ is norm-continuous there, and the series proves norm differentiability with $Q'(\lambda)=-Q(\lambda)^2$. Repeated differentiation gives $Q^{(j)}(\lambda)=(-1)^jj!Q(\lambda)^{j+1}$. Direct subtraction of the inverse equations also yields the [resolvent identity](../../../../../resolvent-identity.md)

$$
Q(\lambda)-Q(\mu)=(\mu-\lambda)Q(\lambda)Q(\mu).
$$

In particular, every [continuous linear functional](../../../../../continuous-linear-functional.md) $\phi$ makes $\phi(Q(\lambda))$ a scalar [holomorphic function](../../../../../holomorphic-function.md); this has been proved, not assumed as an algebra-valued analytic theorem.

The [spectrum of an element](../../../../../spectrum-of-an-element.md) is closed, and is contained in $\{\lambda:|\lambda|\le\|x\|\}$ by the exterior series, so it is compact. It is nonempty. Otherwise $Q$ would be defined and norm-continuous on the entire plane, bounded on every fixed closed disk and tending to zero at infinity. Each $\phi(Q)$ would be a bounded entire scalar function, hence identically zero by [Liouville's theorem](../../../../../liouville-theorem.md). Continuous complex linear functionals separate points of $B$, so $Q(\lambda)=0$, impossible for an inverse. This separation follows from the real [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md): a continuous real functional $h$ not vanishing on a given vector gives the complex linear functional $\phi(v)=h(v)-ih(iv)$, which also does not vanish there. We have therefore proved that

$$
s:=\max_{\lambda\in\sigma(x)}|\lambda|
$$

is well-defined and finite.

Next establish the existence of the power-norm limit. If $x^m=0$ for some $m$, the limit is zero. Otherwise fix $m$ and write $n=qm+r$, $0\le r<m$. Submultiplicativity gives

$$
\|x^n\|\le\|x^m\|^q\|x^r\|.
$$

The finitely many remainder factors have bounded size, and $q/n\to1/m$. Hence $\limsup_n\|x^n\|^{1/n}\le\|x^m\|^{1/m}$ for every $m$. The opposite lower bound by the infimum is automatic, so

$$
r_0:=\lim_n\|x^n\|^{1/n}=\inf_{m\ge1}\|x^m\|^{1/m}.
$$

For $|\lambda|>r_0$, the [root test](../../../../../root-test.md) proves convergence of $\sum x^n/\lambda^{n+1}$ even if $|\lambda|\le\|x\|$. Its finite sums telescope against $\lambda1-x$, and their remainder tends to zero, so this sum is an inverse. Thus $s\le r_0$.

For the reverse inequality, fix $R>s$ and first choose $T>\max(R,\|x\|)$. The exterior [Neumann series](../../../../../neumann-series.md) converges uniformly on $|\lambda|=T$, so termwise vector integration gives

$$
\frac1{2\pi i}\int_{|\lambda|=T}\lambda^nQ(\lambda)\,d\lambda=x^n,\qquad n\ge0.
$$

Only its $x^n\lambda^{-n-1}$ term contributes. The annulus between radii $R$ and $T$ is in the resolvent set. For every continuous complex linear $\phi$, the scalar [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) applied to $\lambda^n\phi(Q(\lambda))$ makes the two contour integrals equal. Continuous linear functionals commute with vector integration and separate points, so the vector integrals themselves agree. This proves the [resolvent Cauchy coefficient formula](../../../../../resolvent-cauchy-coefficient-formula.md) without presupposing any Banach-algebra-valued analytic-function theorem:

$$
x^n=\frac1{2\pi i}\int_{|\lambda|=R}\lambda^nQ(\lambda)\,d\lambda.
$$

Let $M_R=\max_{|\lambda|=R}\|Q(\lambda)\|$, finite by continuity. The contour-length estimate gives $\|x^n\|\le M_RR^{n+1}$. Taking $n$th roots gives $r_0\le R$, and letting $R\downarrow s$ gives $r_0\le s$, including $s=0$. Combined with the earlier inequality, this proves **the spectral radius formula and the corrected printed identity**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
