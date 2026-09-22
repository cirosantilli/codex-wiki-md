<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a positive [Borel measure](../../../../../borel-measure.md) $\nu$, the centered [Hardy-Littlewood maximal function](../../../../../hardy-littlewood-maximal-function.md) and the [uncentered maximal function of a finite measure](../../../../../uncentered-maximal-function-of-a-finite-measure.md) are

$$
m\nu(x)=\sup_{r>0}\frac{\nu(B(x,r))}{|B(x,r)|},\qquad
m_u\nu(x)=\sup_{x\in B(c,r)}\frac{\nu(B(c,r))}{|B(c,r)|}.
$$

We use open balls and allow infinite values. For signed or complex measures the definition uses their [total variation measure](../../../../../variation-measure.md). Since a centered ball is also an admissible uncentered ball, and every ball $B(c,r)$ containing $x$ lies in $B(x,2r)$,

$$
\boxed{m\nu(x)\leq m_u\nu(x)\leq2^d m\nu(x).}
$$

For functions, $m(f)$ means the centered [Hardy-Littlewood maximal function](../../../../../hardy-littlewood-maximal-function.md) of $|f|\,dx$.

The set $E_\alpha$ is the union of the open balls $B$ with $\nu(B)>\alpha|B|$. In particular, each witnessing ball lies entirely inside $E_\alpha$. If $K\subset E_\alpha$ is compact, take a finite witnessing cover of $K$. Choose its largest-radius ball, discard all balls meeting it, and repeat. The selected balls $B_j$ are disjoint. Every discarded ball has no larger radius than the selected ball that discarded it and is contained in its threefold dilation. Hence

$$
|K|\leq3^d\sum_j|B_j|\leq\frac{3^d}{\alpha}\sum_j\nu(B_j)
\leq\frac{3^d}{\alpha}\nu(E_\alpha).
$$

Taking the supremum over compact $K$ by [inner regularity of Lebesgue measure](../../../../../inner-regularity-of-lebesgue-measure.md) proves the stronger, localized estimate

$$
\boxed{|E_\alpha|\leq\frac{3^d}{\alpha}\nu(E_\alpha).}
$$

If the right side is infinite there is nothing to prove. Positivity of the measure is important: a signed version uses $|\nu|(E_\alpha)$, not $\nu(E_\alpha)$.

For the radial-kernel inequality, integrability implies $\phi(r)\to0$. For $0<s<\phi(0)$, let $r(s)$ be the unique radius with $\phi(r(s))=s$. The [layer cake representation](../../../../../layer-cake-representation.md) and [Tonelli theorem](../../../../../tonelli-theorem.md) give

$$
\begin{aligned}
t^{-d}\int\phi(|x-y|/t)|f(y)|\,dy
&=\int_0^{\phi(0)}t^{-d}\int_{B(x,tr(s))}|f(y)|\,dy\,ds\\
&\leq m(f)(x)\int_0^{\phi(0)}v_d r(s)^d\,ds
=m(f)(x).
\end{aligned}
$$

The last integral equals the total mass of $\phi(|\cdot|)$, namely one. Taking the absolute value of the original [convolution](../../../../../convolution.md) therefore proves the claim with constant exactly one. This is [radial decreasing kernel domination by the maximal function](../../../../../radial-decreasing-kernel-domination-by-the-maximal-function.md).

An application is boundary convergence of the [Poisson integral](../../../../../poisson-integral.md). Its normalized radial profile is $c_d(1+r^2)^{-(d+1)/2}$, so $\sup_{t>0}|P_t*f|\leq m(f)$. For a continuous compactly supported $g$, the [approximate identity](../../../../../approximate-identity.md) property gives $P_t*g\to g$ pointwise. For arbitrary $f\in L^1$, put $h=f-g$; then

$$
\limsup_{t\downarrow0}|P_t*f(x)-f(x)|\leq m(h)(x)+|h(x)|.
$$

The preceding [weak type (1,1)](../../../../../weak-type-1-1.md) estimate and the elementary integral bound for $|h|$ show that the set where this exceeds $2a$ has measure at most $(3^d+1)\|h\|_1/a$. Continuous compactly supported functions are dense in $L^1$, so this measure is zero. Thus **the Poisson integrals of an integrable function converge to it almost everywhere**; the same [approximate identity](../../../../../approximate-identity.md) also gives convergence in $L^1$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
