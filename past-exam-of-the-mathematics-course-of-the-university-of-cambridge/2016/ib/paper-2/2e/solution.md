<h1 id="2e/solution">Solution</h1>

↑ **Parent:** [2E](../2e.md)

The [fraction field](../../../../../field-of-fractions.md) of an [integral domain](../../../../../integral-domain.md) $R$ is a [field](../../../../../field.md) $F$ containing an identified copy of $R$ in which every element has the form $a/b$ with $a,b\in R$ and $b\ne0$. Equality means $a/b=c/d$ exactly when $ad=bc$; the operations are the usual addition and multiplication of fractions. We use unital [ring homomorphisms](../../../../../ring-homomorphism.md).

Since $\varphi$ is [injective](../../../../../injective-function.md), $\varphi(b)\ne0$ whenever $b\ne0$. Define

$$
\boxed{\Phi(a/b)=\varphi(a)\varphi(b)^{-1}.}
$$

If $ad=bc$, applying the [ring homomorphism](../../../../../ring-homomorphism.md) and dividing by $\varphi(b)\varphi(d)$ proves the value is independent of the representative. The fraction addition and multiplication rules show that $\Phi$ preserves both operations and one, and $\Phi(a/1)=\varphi(a)$. If $\Phi(a/b)=0$, then $\varphi(a)=0$, so $a=0$ because $\varphi$ is an [injective function](../../../../../injective-function.md); therefore its [kernel](../../../../../kernel-of-a-linear-map.md) is zero and $\Phi$ is [injective](../../../../../injective-function.md). It is also the unique extension, because any [ring homomorphism](../../../../../ring-homomorphism.md) extending $\varphi$ must send $b^{-1}$ to $\varphi(b)^{-1}$.

For a counterexample, take $R=\mathbb Z$, $F=\mathbb Q$, and reduction modulo two $\psi:\mathbb Z\to\mathbb Z/2\mathbb Z$. An extension would give $1=\Psi(2)\Psi(1/2)=0$, a contradiction. **Nonzero denominators must become invertible in the target; an arbitrary ring homomorphism need not have that property.**

## ↑ Ancestors (10)

1. [2E](../2e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
