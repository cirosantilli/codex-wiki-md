<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On $D_+(x_3)$, write $r=x_0/x_3$, $q=x_1/x_3$, and $s=x_2/x_3$. The equations include $q=\pi s^2$ and $r=s^3$; after making these substitutions, the remaining equations are identities. Therefore

$$
\boxed{D_+(x_3)\cong\operatorname{Spec}R[s]=\mathbb A_R^1.}
$$

The other chart is

$$
U=D_+(x_0)=\operatorname{Spec}B,\qquad B=R[a,b,c]/(a^2-\pi^2b,\ ac-\pi b^2,\ ab-\pi c,\ c^2-b^3).
$$

There is a homomorphism $B\to R[t]$ defined by $a\mapsto\pi t$, $b\mapsto t^2$, $c\mapsto t^3$. To prove injectivity rather than merely exhibit a parametrization, reduce monomials using the four relations. Powers of $a$ reduce to at most one $a$; any remaining product of $a$ with $b$ or $c$ eliminates $a$; powers of $c$ reduce to at most one $c$. Thus every element is an $R$-linear combination of

$$
1,\quad a,\quad b^n\ (n\ge1),\quad cb^n\ (n\ge0).
$$

Their images are $1,\pi t,t^{2n},t^{2n+3}$, with pairwise distinct degrees. Since $R$ is a domain and $\pi\ne0$, these images are $R$-linearly independent. Hence they are a [basis](../../../../../../basis.md), the map is injective, and

$$
\boxed{B\cong R[\pi t,t^2,t^3]\subseteq R[t].}
$$

In particular $B$ is torsion-free, indeed free, as an $R$-module.

The two charts cover $X$ by the prime-ideal argument in part i. Both coordinate [rings](../../../../../../ring.md) are torsion-free over the [discrete valuation ring](../../../../../../discrete-valuation-ring.md) $R$, hence flat: over a [principal ideal domain](../../../../../../principal-ideal-domain.md) a [torsion-free module](../../../../../../torsion-free-module.md) is a filtered union of finitely generated free submodules, and filtered colimits preserve flatness. Thus the morphism $X\to\operatorname{Spec}R$ is flat on an open cover and therefore flat everywhere. It is proper because $X$ is a closed subscheme of the proper [projective space](../../../../../../projective-space-split.md) $\mathbb P_R^3$. Consequently **$X$ is both proper and flat over $R$**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 89](../../../paper-89-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
