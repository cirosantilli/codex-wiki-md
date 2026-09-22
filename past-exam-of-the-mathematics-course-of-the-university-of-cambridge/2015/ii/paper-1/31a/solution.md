<h1 id="31a/solution">Solution</h1>

↑ **Parent:** [31A](../31a.md)

Put $C=[A,B]$, which commutes with both operators by hypothesis. Differentiating $e^{\lambda A}Be^{-\lambda A}$ gives $C$, so this conjugate is $B+\lambda C$. Similarly the product $P=e^{\lambda A}e^{\lambda B}$ conjugates $A+B$ to itself: the two central commutator shifts cancel. Hence

$$
F'F^{-1}=A+(B+\lambda C)-(A+B)=\lambda C.
$$

With $F(0)=I$, the operator differential equation gives $F(\lambda)=e^{\lambda^2C/2}$. At $\lambda=1$ this proves the central-commutator [Baker--Campbell--Hausdorff formula](../../../../../baker-campbell-hausdorff-formula.md)

$$
\boxed{e^Ae^B=e^{[A,B]/2}e^{A+B}}.
$$

These formal manipulations apply on a suitable common domain, or to the oscillator exponentials below where the corresponding unitary identities are well defined.

The oscillator has $[a,a^\dagger]=1$ and $H=\hbar\omega(a^\dagger a+1/2)$. Its normalized states and energies are

$$
\boxed{|n\rangle=\frac{(a^\dagger)^n}{\sqrt{n!}}|0\rangle,\qquad E_n=\hbar\omega(n+1/2)}.
$$

Since $\hat x=\sqrt{\hbar/(2m\omega)}(a+a^\dagger)$, put $\gamma=\mu\sqrt{\hbar/(2m\omega)}$. Taking $A=\pm i\gamma a^\dagger$, $B=\pm i\gamma a$ gives $[A,B]=\gamma^2$. The formula implies $e^{\pm i\mu\hat x}=e^{-\gamma^2/2}e^{\pm i\gamma a^\dagger}e^{\pm i\gamma a}$. Averaging the two signs proves the requested [normal ordering](../../../../../normal-ordering.md) of the cosine.

Because $a|0\rangle=0$, expansion of the remaining creation exponential gives

$$
\langle n|V|0\rangle=e^{-\gamma^2/2}\frac{(i\gamma)^n+(-i\gamma)^n}{2\sqrt{n!}}.
$$

Odd [matrix](../../../../../matrix.md) elements vanish, the ground expectation is $e^{-\gamma^2/2}$, and the magnitude squared for $n=2p$ is $e^{-\gamma^2}\gamma^{4p}/(2p)!$. The nondegenerate [second-order nondegenerate perturbation theory](../../../../../second-order-nondegenerate-perturbation-theory.md) formula is $\Delta E_0=\epsilon V_{00}+\epsilon^2\sum_{n>0}|V_{n0}|^2/(E_0-E_n)+O(\epsilon^3)$. Therefore

$$
\boxed{\Delta E_0=\epsilon e^{-\mu^2\hbar/(4m\omega)}-
\frac{\epsilon^2e^{-\mu^2\hbar/(2m\omega)}}{\hbar\omega}
\sum_{p=1}^\infty\frac{(\mu^2\hbar/(2m\omega))^{2p}}{(2p)!(2p)}+O(\epsilon^3)}.
$$

The negative second-order sign comes from the higher unperturbed energies in every denominator.

## ↑ Ancestors (10)

1. [31A](../31a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
