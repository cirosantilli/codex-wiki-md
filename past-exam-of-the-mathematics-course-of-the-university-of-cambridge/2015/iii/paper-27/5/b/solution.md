<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Finite rearrangement and the [Von Mangoldt divisor identity](../../../../../../von-mangoldt-divisor-identity.md) give

$$
T(x)=\sum_{n\leq x}\sum_{m\leq x/n}\Lambda(m)
=\sum_{k\leq x}\sum_{m\mid k}\Lambda(m)
=\sum_{k\leq x}\log k=\log(\lfloor x\rfloor!).
$$

For $m=\lfloor x\rfloor$, integral comparison of the increasing [logarithm](../../../../../../logarithm.md) gives $\log(m!)=m\log m-m+O(\log(m+1))$. Moving $m$ to real $x$ changes the main term by $O(\log(x+1))$. Thus the [integrated Chebyshev sum](../../../../../../integrated-chebyshev-sum.md) has

$$
\boxed{T(x)=x\log x-x+O(\log(x+1))\quad(x\geq1).}
$$

For $x\geq2$, choose

$$
\lambda_d=\frac{\mu(d)\log(x/d)}{\log x}\quad(d\leq x),\qquad\lambda_d=0\quad(d>x).
$$

These are logarithmic [Möbius function](../../../../../../mobius-function.md) weights; they need not be [upper-bound sieve](../../../../../../upper-bound-sieve.md) weights. For $n\leq x$, the [Möbius inversion](../../../../../../mobius-inversion-formula.md) identities $\mu*\mathbf1=\epsilon$ and $\mu*\log=\Lambda$ give

$$
\sum_{d\mid n}\lambda_d=1_{n=1}+\frac{\Lambda(n)}{\log x}.
$$

Hence the expression suggested in the question is

$$
F(x)=\sum_{n\leq x}\psi(x/n)\sum_{d\mid n}\lambda_d
=\psi(x)+\frac1{\log x}\sum_{n\leq x}\Lambda(n)\psi(x/n)
=\frac1{\log x}\sum_{d\leq x}\mu(d)\log(x/d)T(x/d).
$$

We will use the elementary [Möbius harmonic logarithmic moments](../../../../../../mobius-harmonic-logarithmic-moments.md), $A_j(x)=\sum_{d\leq x}\mu(d)\log^j(x/d)/d$, for which

$$
A_0(x)=O(1),\qquad A_1(x)=O(1),\qquad A_2(x)=2\log x+O(1).
$$

Here is a proof of the needed estimates. From $\sum_d\mu(d)\lfloor x/d\rfloor=1$, replacing floors by $x/d+O(1)$ gives $A_0=O(1)$. Also $\sum_d\mu(d)H_{\lfloor x/d\rfloor}/d=1$, because $\mu*\mathbf1=\epsilon$. Substituting the permitted [harmonic number](../../../../../../harmonic-number.md) estimate $H_{\lfloor t\rfloor}=\log t+\gamma+O(1/t)$ gives $A_1+\gamma A_0=1+O(1)$, so $A_1=O(1)$.

For $A_2$, the weighted [Dirichlet hyperbola method](../../../../../../dirichlet-hyperbola-method.md) gives the [harmonic divisor sum](../../../../../../harmonic-divisor-sum.md) expansion

$$
B(t)=\sum_{m\leq t}\frac{\tau(m)}m
=\tfrac12\log^2t+2\gamma\log t+c+O\left(\frac{\log(2t)}{\sqrt t}\right).
$$

Explicitly, for $r=\lfloor\sqrt t\rfloor$, $B(t)=2\sum_{a\leq r}H_{\lfloor t/a\rfloor}/a-H_r^2$. Substitute the harmonic estimate and $\sum_{a\leq r}(\log a)/a=\tfrac12\log^2r+c\prime+O(\log(2r)/r)$, obtained by unit-interval integral comparison. This proves the expansion without a prime-distribution theorem. Since $\tau=\mathbf1*\mathbf1$, we have $\mu*\tau=\mathbf1$, and therefore

$$
\sum_{d\leq x}\frac{\mu(d)}dB(x/d)=H_{\lfloor x\rfloor}
=\tfrac12A_2+2\gamma A_1+cA_0+O(1).
$$

The summed error is bounded by $x^{-1/2}\sum_{d\leq x}d^{-1/2}\log(2x/d)=O(1)$, by integral comparison. Thus $A_2=2\log x+O(1)$.

Finally substitute the asymptotic for $T$ into $F$. The main term is

$$
F(x)=\frac{x}{\log x}\bigl(A_2(x)-A_1(x)\bigr)
+O\left(\frac1{\log x}\sum_{d\leq x}\log(x/d)\log(x/d+1)\right).
$$

The error [sum](../../../../../../sum.md) is $O(x)$: partition the integers $d$ into $x/2^{j+1}<d\leq x/2^j$; each interval contributes $O(x(j+1)^2/2^j)$, and the resulting series converges. Using the moment estimates proves the [Selberg symmetry formula](../../../../../../selberg-symmetry-formula.md):

$$
\boxed{\psi(x)+\sum_{n\leq x}\psi(x/n)\frac{\Lambda(n)}{\log x}=2x+O\left(\frac{x}{\log x}\right).}
$$

In particular, the factor two comes from the quadratic logarithmic moment, rather than from an assumption of the [Prime number theorem](../../../../../../prime-number-theorem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
