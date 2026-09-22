<h1 id="mobius-harmonic-logarithmic-moments">Möbius harmonic logarithmic moments</h1>

↑ **Parent:** [Möbius function](mobius-function.md)

Put $A_j(x)=\sum_{d\leq x}\mu(d)\log^j(x/d)/d$. The elementary estimates are

$$
A_0(x)=O(1),\qquad A_1(x)=O(1),\qquad A_2(x)=2\log x+O(1).
$$

The identities $\sum_d\mu(d)\lfloor x/d\rfloor=1$ and $\sum_d\mu(d)H_{\lfloor x/d\rfloor}/d=1$ give the first two bounds. Convolve the [harmonic divisor sum](harmonic-divisor-sum.md) with $\mu(d)/d$: because $\mu*\tau=\mathbf1$, its left side is $H_{\lfloor x\rfloor}$. Thus $\tfrac12A_2+2\gamma A_1+cA_0=\log x+O(1)$. The summed error is $O(x^{-1/2}\sum_{d\leq x}d^{-1/2}\log(2x/d))=O(1)$.

This elementary smoothing argument is used in [Selberg's original proof](https://www.math.lsu.edu/~mahlburg/teaching/handouts/2014-7230/Selberg-ElemPNT1949.pdf) and [Ramaré's sieve lectures, Lemma 4.2](https://ramare-olivier.github.io/Maths/LecturesEasyChennai.pdf).

## ↑ Ancestors (6)

1. [Möbius function](mobius-function.md)
2. [Arithmetic function](arithmetic-function.md)
3. [Number theory](number-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-27/5/b/solution.md)
- [Selberg symmetry formula](selberg-symmetry-formula.md)
