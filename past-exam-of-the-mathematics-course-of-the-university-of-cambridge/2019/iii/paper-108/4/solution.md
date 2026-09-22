<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a finite partition $\xi$, put

$$
\mathcal F_n(\xi)=\bigvee_{k=n}^{\infty}T^{-k}\xi.
$$

The system is [K-mixing](../../../../../k-mixing.md) when every measurable $A$ becomes uniformly asymptotically independent of this remote future:

$$
\sup_{B\in\mathcal F_n(\xi)}|\mu(A\cap B)-\mu(A)\mu(B)|\longrightarrow0.
$$

Taking $\xi=\{B,X\setminus B\}$ makes $T^{-n}B\in\mathcal F_n(\xi)$, so

$$
\mu(A\cap T^{-n}B)\longrightarrow\mu(A)\mu(B).
$$

Thus **K-mixing implies mixing**.

The [tail sigma-algebra of a measurable partition](../../../../../tail-sigma-algebra-of-a-measurable-partition.md) is

$$
\mathcal T(\xi)=\bigcap_{n\geq0}\mathcal F_n(\xi).
$$

By the [reverse martingale convergence theorem](../../../../../reverse-martingale-convergence-theorem.md),

$$
\mathbb E[\mathbf1_A\mid\mathcal F_n(\xi)]
\longrightarrow
\mathbb E[\mathbf1_A\mid\mathcal T(\xi)]
$$

in $L^1$. The uniform independence in the definition of K-mixing is equivalent to the limit being the constant $\mu(A)$ for every $A$. This holds exactly when every $\mathcal T(\xi)$-measurable set has measure zero or one. Hence the system is K-mixing if and only if every finite partition has trivial tail sigma-algebra.

Let $\mathcal P=\{A:h_\mu(T,\xi_A)=0\}$. Complements preserve the binary partition. If $A,B\in\mathcal P$, then $\xi_{A\cup B}$ is coarser than $\xi_A\vee\xi_B$, so subadditivity gives zero entropy rate. Thus $\mathcal P$ is an algebra. For $A=\bigcup_{j\geq1}A_j$, let $A^{(m)}=\bigcup_{j\leq m}A_j$. The entropy metric continuity bound

$$
|h_\mu(T,\xi_A)-h_\mu(T,\xi_{A^{(m)}})|
\leq H_\mu(\xi_A\mid\xi_{A^{(m)}})+H_\mu(\xi_{A^{(m)}}\mid\xi_A)
$$

tends to zero because $\mu(A\mathbin\triangle A^{(m)})\to0$. Hence $A\in\mathcal P$, proving that $\mathcal P$ is a sigma-algebra: the [Pinsker sigma-algebra](../../../../../pinsker-sigma-algebra.md).

If $A$ belongs modulo null sets to $\mathcal T(\xi)$ for a finite $\xi$, remote-future approximations make the entropy rate of $\xi_A$ zero. Conversely, if $h_\mu(T,\xi_A)=0$, the conditional-entropy formula for entropy rate gives

$$
H_\mu\left(\xi_A\,middle|\,\bigvee_{n=1}^{\infty}T^{-n}\xi_A\right)=0.
$$

Thus $A$ is measurable modulo null sets from its strict future. Iterating this fact makes it measurable from every remote future, so $A\in\mathcal T(\xi_A)$ modulo null sets. Therefore

$$
\boxed{A\in\mathcal P\iff
\exists\text{ finite }\xi\ \exists A'\in\mathcal T(\xi):
\mu(A\mathbin\triangle A')=0.}
$$

This is the [Tail characterization of the Pinsker sigma-algebra](../../../../../tail-characterization-of-the-pinsker-sigma-algebra.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 108](../../paper-108-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
