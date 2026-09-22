<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

Call a set function $f$ with [ordinal](../../../../../ordinal.md) domain $\gamma$ good if $f(\xi)=G(\xi,\operatorname{ran}(f|_\xi))$ for every $\xi<\gamma$. Any two good functions agree on their common domain: otherwise their first disagreement has identical earlier ranges and hence identical values under $G$. This is [transfinite induction](../../../../../transfinite-induction.md), not an assumption of the desired recursion.

Good functions exist with every [ordinal](../../../../../ordinal.md) domain. At a successor stage extend the unique previous function by its prescribed value under $G$. At a limit stage, [Axiom schema of replacement](../../../../../axiom-schema-of-replacement.md) collects the unique good functions on all smaller domains into a set, and their compatible union is a good function on the limit domain. Each earlier range is a set, so $G$ is applied only to sets. [Transfinite induction](../../../../../transfinite-induction.md) now establishes existence at all stages. Define $F(\alpha)$ to be the value at $\alpha$ of the unique good function on $\alpha+1$. This is a definable class function because goodness and the uniqueness assertion are formulas in the defining formula for $G$. Compatibility gives

$$
\boxed{F(\alpha)=G(\alpha,\{F(\beta):\beta<\alpha\}).}
$$

An [initial ordinal](../../../../../initial-ordinal.md) is an [ordinal](../../../../../ordinal.md) not bijective with any smaller [ordinal](../../../../../ordinal.md). It is the canonical [ordinal](../../../../../ordinal.md) representative of a well-orderable [cardinal](../../../../../cardinal-number.md), so [cardinal arithmetic](../../../../../cardinal-arithmetic.md) can be defined by taking the [initial ordinal](../../../../../initial-ordinal.md) equinumerous with a disjoint union, Cartesian product or function set. In the usual setting with the [axiom of choice](../../../../../axiom-of-choice.md), every cardinal has such a representative. [Hartogs theorem](../../../../../hartogs-theorem.md) says that for every set $A$ there is an [ordinal](../../../../../ordinal.md) $h(A)$ which does not inject into $A$, and there is a least such [ordinal](../../../../../ordinal.md). For an [initial ordinal](../../../../../initial-ordinal.md) $\kappa$ it is the next larger [initial ordinal](../../../../../initial-ordinal.md): every smaller [ordinal](../../../../../ordinal.md) injects into $\kappa$, and if $h(\kappa)$ were equinumerous with a smaller [ordinal](../../../../../ordinal.md) it too would inject into $\kappa$.

Use the recursion just proved to set $\omega_0=\omega$, $\omega_{\beta+1}=h(\omega_\beta)$ and $\omega_\lambda=\sup_{\beta<\lambda}\omega_\beta$ for nonzero limit $\lambda$. These instructions use the earlier value set alone: at a successor it has a maximum, and at a limit its supremum is taken. They are therefore implemented by an appropriate definable $G$. The limit supremum is initial: if it were bijective with $\gamma$ below it, choose an earlier $\omega_\beta>\gamma$; then $\omega_\beta$ would inject into $\gamma$, contradicting initiality. The sequence is strictly increasing and continuous. There are no omitted infinite [initial ordinals](../../../../../initial-ordinal.md), since each successor chooses the least next one and each limit is the supremum; more formally, a least omitted [initial ordinal](../../../../../initial-ordinal.md) cannot lie between successive terms, and the least term above it cannot be a limit term. Terms eventually exceed any prescribed [ordinal](../../../../../ordinal.md), since a strictly increasing [ordinal](../../../../../ordinal.md) sequence satisfies $\omega_\beta\geq\beta$.

There is a [fixed point of a normal ordinal function](../../../../../fixed-point-of-a-normal-ordinal-function.md). Explicitly let $\alpha_0=0$, $\alpha_{n+1}=\omega_{\alpha_n}$ and $\alpha=\sup_{n<\omega}\alpha_n$. The sequence is strictly increasing, by induction from $0<\omega_0$ and strict increase of the enumeration. It is cofinal in the limit $\alpha$, so continuity gives

$$
\boxed{\omega_\alpha=\sup_n\omega_{\alpha_n}=\sup_n\alpha_{n+1}=\alpha.}
$$

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
