<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $K=\mathbb C((t))$. This is a complete [discretely valued field](../../../../../../discretely-valued-field.md), with valuation ring $\mathbb C[[t]]$ and residue field $\mathbb C$; its infinite residue field means it is not a locally compact [local field](../../../../../../local-field.md). The finite-extension facts needed here are uniqueness of the extended valuation, completeness of the extension, and $[L:K]=ef$ for complete discretely valued fields with perfect residue field. They apply in this characteristic-zero setting.

Let $[L:K]=n$. The finite residue extension of $\mathbb C$ must be $\mathbb C$ itself, so $f=1$ and $e=n$. Normalize $v_L$ integrally and choose a [uniformizer](../../../../../../uniformizer.md) $\pi$. Since $v_L(t)=n$, write $t=u\pi^n$ with $u\in\mathcal O_L^\times$.

The residue of $u$ has an $n$th root $b_0\in\mathbb C^\times$. Apply [Hensel lemma](../../../../../../hensel-s-lemma.md) to $X^n-u$: its derivative at $b_0$ is the unit $nb_0^{n-1}$ because the residue characteristic is zero. Hence there is $v\in\mathcal O_L^\times$ with $v^n=u$. Setting $s=v\pi$ gives

$$
s^n=t,\qquad v_L(s)=1.
$$

The elements $1,s,\ldots,s^{n-1}$ are linearly independent over $K$. In a nontrivial relation $\sum_{i=0}^{n-1}a_is^i=0$, the nonzero summands have valuations $nv_K(a_i)+i$, distinct modulo $n$, so exactly one has least valuation and cannot cancel. Since $L$ has dimension $n$, this proves $L=K(s)$.

The constants already embed $\mathbb C$ into $\mathcal O_L$ with residue field $\mathbb C$. Subtracting the residue coefficient and dividing by $s$ repeatedly, exactly as in Question 1(c), expresses every integral element uniquely as $\sum_{j\ge0}c_js^j$ with $c_j\in\mathbb C$. Completeness and the first-nonzero-coefficient valuation show that allowing finite negative powers gives

$$
\boxed{L\cong\mathbb C((s))=\mathbb C((t^{1/n})),\qquad t=s^n.}
$$

This proof of [finite extensions of the complex Laurent series field](../../../../../../finite-extensions-of-the-complex-laurent-series-field.md) did not need a Galois hypothesis. All $n$ distinct $n$th roots of unity lie in the constant field, and the substitutions $s\mapsto\zeta s$ preserve $s^n=t$. They give all $n$ automorphisms, so every such finite extension is cyclic Galois:

$$
\operatorname{Gal}(L/K)\cong\mu_n\cong\mathbb Z/n\mathbb Z.
$$

Choose compatible roots $s_n=t^{1/n}$ in an algebraic closure, first choosing them successively along the factorial-degree tower and then taking powers to define the other roots, with $s_n=s_m^{m/n}$ whenever $n\mid m$. The fields $K_n=K(s_n)$ are nested under divisibility. Every finite extension inside the closure equals one of them: its constructed root $s$ of $X^n-t$ differs from $s_n$ by a constant root of unity. Therefore their union is the entire algebraic closure. Explicitly, every algebraic element generates a finite extension, so lies in the union; any polynomial over the union has its coefficients in one finite extension, and its roots are still algebraic over $K$, hence also lie there.

For $n\mid m$, restriction of automorphisms sends $\zeta_m\in\mu_m$ to $\zeta_m^{m/n}\in\mu_n$. Using the compatible primitive roots $\exp(2\pi i/n)$, these are the reduction maps on exponent groups. Thus the [absolute Galois group of the complex Laurent series field](../../../../../../absolute-galois-group-of-the-complex-laurent-series-field.md) is

$$
\boxed{\operatorname{Gal}(\overline{\mathbb C((t))}/\mathbb C((t)))\cong\varprojlim_n\mathbb Z/n\mathbb Z=\widehat{\mathbb Z}\cong\prod_{\ell\text{ prime}}\mathbb Z_\ell.}
$$

The [inverse limit](../../../../../../inverse-limit.md) carries its profinite topology; choosing compatible roots gives the displayed identification with the [profinite completion](../../../../../../profinite-completion.md) of the integers.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
