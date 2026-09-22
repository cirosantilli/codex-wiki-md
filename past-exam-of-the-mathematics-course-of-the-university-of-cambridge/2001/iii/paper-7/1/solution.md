<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the common nonzero identity $1$. If $\|h\|<1$, [completeness](../../../../../completeness.md) and [submultiplicativity](../../../../../submultiplicativity.md) give the [Neumann series](../../../../../neumann-series.md)

$$
(1-h)^{-1}=\sum_{n=0}^\infty h^n.
$$

For $a\in G(A)$ and $\|a^{-1}\|\|b-a\|<1$, write $b=a(1+a^{-1}(b-a))$ and apply that series. This proves that the [group of invertible elements of a Banach algebra](../../../../../group-of-invertible-elements-of-a-banach-algebra.md) is [open](../../../../../open-set.md). Locally the same series bounds $\|b^{-1}\|$, and

$$
b^{-1}-a^{-1}=b^{-1}(a-b)a^{-1}
$$

proves [continuity](../../../../../continuous-function.md) of inversion. Inversion is its own inverse, hence **it is a [homeomorphism](../../../../../homeomorphism.md) of $G(A)$ onto itself**.

The [spectrum of an element](../../../../../spectrum-of-an-element.md) is $\sigma_A(x)=\{\lambda:\lambda1-x\notin G(A)\}$, and its complement is the [algebra resolvent set](../../../../../resolvent-set-of-a-banach-algebra-element.md) $\rho_A(x)$. Openness of $G(A)$ makes the [algebra spectrum](../../../../../spectrum-of-an-element.md) [closed](../../../../../closed-set.md). For $|\lambda|>\|x\|$,

$$
R(\lambda)=(\lambda1-x)^{-1}=\frac1\lambda\sum_{n=0}^\infty(x/\lambda)^n,
$$

so it is bounded and thus [compact](../../../../../compact-space.md). For nonemptiness, suppose $R$ existed everywhere. The local Neumann expansion around each point makes $R$ a Banach-space-valued [entire function](../../../../../entire-function.md). For every [bounded linear functional](../../../../../continuous-linear-functional.md) $\ell$ on $A$, $\ell(R(\lambda))$ is entire, bounded on [compact](../../../../../compact-space.md) discs, and tends to zero at infinity by the displayed series. The [Liouville theorem](../../../../../liouville-theorem.md) makes it identically zero. The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) separates points, so $R(\lambda)=0$, contradicting $(\lambda1-x)R(\lambda)=1$. Hence **the [algebra spectrum](../../../../../spectrum-of-an-element.md) is nonempty and [compact](../../../../../compact-space.md)**.

If $B$ is a [closed](../../../../../closed-set.md) [unital](../../../../../unital-algebra.md) subalgebra with the same identity, then $\rho_B(x)\subseteq\rho_A(x)$. It is relatively [open](../../../../../open-set.md) by the [Neumann series](../../../../../neumann-series.md) in $B$. If $\lambda_j\in\rho_B(x)$ tends to $\lambda\in\rho_A(x)$, [continuity](../../../../../continuous-function.md) of inversion in $A$ gives $(\lambda_j1-x)^{-1}\to(\lambda1-x)^{-1}$. Closedness puts this last inverse in $B$, so $\lambda\in\rho_B(x)$. Therefore **$\rho_B(x)$ is relatively [open](../../../../../open-set.md) and [closed](../../../../../closed-set.md) in $\rho_A(x)$**. This proves the required [resolvent components in a closed unital subalgebra](../../../../../resolvent-components-in-a-closed-unital-subalgebra.md) directly, with no spectral-boundary assumption.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
