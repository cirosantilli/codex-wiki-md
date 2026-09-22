<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix a prime $\mathfrak q$ of $E$ over $\mathfrak p$, and a prime $\mathfrak r$ of $LE$ over $\mathfrak q$. Let $\mathfrak P$ be its restriction to $L$. Inside the completed compositum, put

$$
F=K_{\mathfrak p},\qquad J=E_{\mathfrak q},\qquad U=L_{\mathfrak P}.
$$

The assumption means $U/F$ is an [unramified extension](../../../../../../unramified-extension.md). Its [residue degree](../../../../../../residue-degree.md) is some $f$; the completed extension $(LE)_{\mathfrak r}/J$ is the corresponding compositum $UJ/J$. It suffices to prove that this is [unramified](../../../../../../unramified-extension.md), regardless of the [ramification](../../../../../../ramification-mathematics.md) of $J/F$.

Here is a proof of [unramified extensions remain unramified under base change](../../../../../../unramified-extensions-remain-unramified-under-base-change.md) using the classification already established. Choose an integral generator $\alpha$ of $U/F$ whose monic [minimal polynomial](../../../../../../minimal-polynomial.md) $g\in\mathcal O_F[X]$ has irreducible separable reduction of degree $f$. Write $k_F=\mathbb F_q$ and $k_J=\mathbb F_{q^r}$. Let $J_f/J$ be the degree-$f$ [unramified extension](../../../../../../unramified-extension.md). Its [residue field](../../../../../../residue-field.md) $\mathbb F_{q^{rf}}$ contains $\mathbb F_{q^f}$, so $\bar g$ has a simple root there. [Hensel lemma](../../../../../../hensel-s-lemma.md) lifts this root to a root of $g$ in $J_f$. This gives an $F$-embedding $U\hookrightarrow J_f$.

An [unramified extension](../../../../../../unramified-extension.md) of a [local field](../../../../../../local-field.md) is [Galois](../../../../../../finite-galois-extension.md), so all $F$-embeddings of $U$ into a fixed algebraic closure have the same image. The original $U$ therefore lies in $J_f$, and $UJ$ is an intermediate field of the [unramified extension](../../../../../../unramified-extension.md) $J_f/J$. Its [ramification index](../../../../../../ramification-index.md) is one. Since $\mathfrak q$ and $\mathfrak r$ were arbitrary,

$$
\boxed{e(\mathfrak r/\mathfrak q)=1\text{ for every prime above }\mathfrak p.}
$$

This proof also explains why no linear-disjointness assumption on $L$ and $E$, and no assumption that $E/K$ is [unramified](../../../../../../unramified-extension.md), is needed.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
