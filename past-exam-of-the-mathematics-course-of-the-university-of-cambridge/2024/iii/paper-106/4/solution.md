<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $M^+(K)$ be the positive linear functionals on $C(K)$: those $\varphi$ for which $f\geq0$ implies $\varphi(f)\geq0$. For real $f$,

$$
-\|f\|_\infty1_K\leq f\leq\|f\|_\infty1_K,
$$

so positivity gives $|\varphi(f)|\leq\varphi(1_K)\|f\|_\infty$; decomposition into real and imaginary parts, or the positive-functional Cauchy--Schwarz inequality, gives the same bound for complex $f$. Hence $\varphi$ is continuous and

$$
\boxed{\|\varphi\|=\varphi(1_K)}.
$$

The [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md) says that there is a unique finite regular positive Borel measure $\mu$ with

$$
\varphi(f)=\int_Kf\,d\mu.
$$

More generally, $C(K)^*=M(K)$ is the Banach space of finite regular complex Borel measures with the total-variation norm.

Now let $A\subseteq\mathcal B(H)$ be commutative, unital, and C-star, and put $K=\Phi_A$. The [Gelfand transform](../../../../../gelfand-representation.md) is an isometric star-isomorphism $A\cong C(K)$. For $\xi,\eta\in H$, the functional

$$
\widehat T\longmapsto\langle T\xi,\eta\rangle
$$

on $C(K)$ is represented by a regular complex measure $\mu_{\xi,\eta}$. The diagonal measures are positive. Polarization and the Riesz theorem assemble them into a projection-valued measure $E$ characterized by

$$
\langle E(S)\xi,\eta\rangle=\mu_{\xi,\eta}(S)
$$

for Borel sets $S\subseteq K$. The multiplication identities first hold for continuous functions and extend to bounded Borel functions by a monotone-class argument. Therefore

$$
\Psi(f)=\int_Kf\,dE,
\qquad f\in L^\infty(K),
$$

defines a unital star-homomorphism with $\|\Psi(f)\|\leq\|f\|_\infty$, and

$$
\Psi(\widehat T)=T
$$

for every $T\in A$.

For a normal $T\in\mathcal B(H)$, apply this construction to the commutative C-star algebra $C^*(1,T)$. Its character space identifies with $\sigma(T)$, and the [Gelfand transform](../../../../../gelfand-representation.md) of $T$ is the coordinate function $z(\lambda)=\lambda$. We obtain the [Borel functional calculus for a normal operator](../../../../../borel-functional-calculus-for-a-normal-operator.md)

$$
\Psi:L^\infty(\sigma(T))\to\mathcal B(H),
\qquad
\Psi(z)=T.
$$

If $\sigma(T)\subseteq\mathbb T$, then $\overline z,z=z\overline z=1$ on the spectrum. Since $\Psi$ preserves products and involution,

$$
T^*T=\Psi(\overline z)\Psi(z)=I,
\qquad
TT^*=I.
$$

**Thus $T$ is a [unitary operator](../../../../../unitary-element-of-a-c-star-algebra.md).**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
