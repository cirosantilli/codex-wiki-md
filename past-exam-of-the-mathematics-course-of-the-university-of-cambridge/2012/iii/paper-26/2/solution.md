<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $\Gamma=\operatorname{Gal}(K_\infty/K)\cong\mathbb Z_p$. Its only finite subgroup is trivial. In particular, a real place cannot acquire complex inertia in this [Zp-extension](../../../../../zp-extension.md): the possible nontrivial inertia at a real place has order two. Thus every infinite place splits in the tower.

Suppose that no finite prime ramified. Every finite layer would then be an abelian [everywhere unramified extension of number fields](../../../../../everywhere-unramified-extension-of-number-fields.md), including splitting at real places. Every layer would lie in the ordinary [Hilbert class field](../../../../../hilbert-class-field.md) of $K$, a finite extension. Their degrees are unbounded, a contradiction. Therefore **some finite prime must ramify**.

Let $v$ have residue characteristic $\ell\ne p$. Apply [local class field theory](../../../../../local-class-field-theory.md) to the corresponding [decomposition group](../../../../../decomposition-group.md), a closed subgroup of $\Gamma$. The image of the unit group $\mathcal O_{K_v}^\times$ is the [inertia group](../../../../../inertia-group.md). Its first principal-unit subgroup is a [pro-l group](../../../../../pro-p-group.md), so its continuous image in the [pro-p group](../../../../../pro-p-group.md) $\Gamma$ is trivial. The residue-unit quotient is the finite group $\mathbb F_{q_v}^\times$. Its image is finite, and is therefore also trivial in the torsion-free group $\mathbb Z_p$. The entire [inertia group](../../../../../inertia-group.md) is trivial. Hence

$$
\boxed{v\text{ ramifies in }K_\infty/K\ \Longrightarrow\ v\mid p.}
$$

Equivalently, the [tame ramification](../../../../../tamely-ramified-extension.md) relation with a Frobenius element would force a tame inertia generator to satisfy $\tau^{q_v-1}=1$, which is impossible nontrivially in $\mathbb Z_p$.

For the final assertion, the [cyclotomic Zp-extension](../../../../../cyclotomic-zp-extension.md) of $K$ is $K\mathbb Q[p^\infty]$. Fix $v\mid p$ and put $E=K_v$, a finite extension of $\mathbb Q_p$. Let $C_n$ be the completion of $\mathbb Q[p^n]$ at its unique prime over $p$. This is a [totally ramified extension](../../../../../totally-ramified-extension.md) of $\mathbb Q_p$ of degree $p^n$. In a compatible local algebraic closure,

$$
e(EC_n/E)
=\frac{e(EC_n/\mathbb Q_p)}{e(E/\mathbb Q_p)}
\geq\frac{p^n}{e(E/\mathbb Q_p)}.
$$

Here the inequality follows from the tower through $C_n$. The right side is unbounded. These composita occur among the completions of the cyclotomic tower over $K$, so $v$ has unbounded [ramification index](../../../../../ramification-index.md), in particular nontrivial [inertia group](../../../../../inertia-group.md). Thus

$$
\boxed{\text{Every prime }v\mid p\text{ ramifies in the cyclotomic Zp-extension.}}
$$

This argument allows an arbitrary finite intersection between $K$ and the rational cyclotomic tower; it does not assume disjointness.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
