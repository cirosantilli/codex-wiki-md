<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Fix a separable closure $k^s$. The [Tate module](../../../../../tate-module.md) and [rational Tate module](../../../../../rational-tate-module.md) are

$$
T_\ell(E)=\varprojlim_n E[\ell^n](k^s),\qquad V_\ell(E)=T_\ell(E)\otimes_{\mathbb Z_\ell}\mathbb Q_\ell,
$$

where the transition maps are multiplication by $\ell$. Since $\ell$ is different from the characteristic, $E[\ell^n](k^s)\simeq(\mathbb Z/\ell^n)^2$ and these transition maps are surjective. Choosing compatible bases gives $T_\ell(E)\simeq\mathbb Z_\ell^2$, and $T_\ell(E)/\ell^nT_\ell(E)\simeq E[\ell^n]$. Both spaces carry the natural continuous action of the [absolute Galois group](../../../../../absolute-galois-group.md) of $k$ and of the base-defined [endomorphism ring of an elliptic curve](../../../../../endomorphism-ring-of-an-elliptic-curve.md).

For **(i)**, choose a nonrational $a\in R$. Such an element exists because the intersection of the given two-dimensional rational subalgebra with the integral [endomorphism ring](../../../../../endomorphism-ring.md) contains a full lattice. The characteristic equation of an elliptic [endomorphism](../../../../../endomorphism.md) is

$$
a^2-\operatorname{tr}(a)a+\deg(a)=0.
$$

Since $a\in K$ is nonrational, its minimal polynomial over $\mathbb Q$ has degree two. Comparing the two monic equations gives $\operatorname{tr}(a)=a+\bar a$ and $\deg(a)=a\bar a$. The same is the characteristic polynomial on the [rational Tate module](../../../../../rational-tate-module.md): the [Weil pairing](../../../../../weil-pairing.md) gives determinant $\deg(a)$, and applying it to $1-a$ gives trace $1+\deg(a)-\deg(1-a)$. Thus on $V_\ell(E)$ the characteristic polynomial is

$$
(X-a)(X-\bar a).
$$

If $K_\ell$ is a quadratic [field](../../../../../field.md) over $\mathbb Q_\ell$, a unital $K_\ell$-action on this two-dimensional $\mathbb Q_\ell$-space makes it a one-dimensional $K_\ell$-space. If $K_\ell\simeq\mathbb Q_\ell\times\mathbb Q_\ell$, the two roots above are distinct in $\mathbb Q_\ell$ and their eigenspaces each have dimension one. The two idempotent factors therefore have equal rank one, so the [module](../../../../../module-mathematics.md) is again free of rank one. This also proves faithfulness in the split case. Hence

$$
\boxed{V_\ell(E)\simeq K_\ell\quad\text{as }K_\ell\text{-modules}.}
$$

For **(ii)**, first prove an integral divisibility statement. If $a\in R$ maps $T_\ell(E)$ into $\ell^nT_\ell(E)$, then its induced action on $E[\ell^n]$ is zero. The [kernel of an isogeny](../../../../../kernel-of-an-isogeny.md) of $[\ell^n]$ is therefore contained in the kernel of $a$. The quotient property of this [isogeny of elliptic curves](../../../../../isogeny-of-elliptic-curves.md) gives a unique [endomorphism](../../../../../endomorphism.md) $b$ with

$$
a=b\circ[\ell^n]=[\ell^n]\circ b.
$$

This factorization is defined over $k$: applying any descent automorphism preserves it, and uniqueness fixes $b$. Inside the rational [endomorphism ring](../../../../../endomorphism-ring.md), $b=a/\ell^n$ belongs to $K$, so $b\in R$. Consequently

$$
\{a\in R:aT_\ell(E)\subseteq\ell^nT_\ell(E)\}=\ell^nR.
$$

Here the prime-to-characteristic torsion is étale, so vanishing on its geometric points is vanishing on the entire kernel scheme.

Every element of $R_\ell$ preserves the [Tate module](../../../../../tate-module.md) by continuity. Conversely suppose $\phi\in K_\ell$ preserves it. Choose $n\geq0$ with $\ell^n\phi\in R_\ell$, and approximate it by $a\in R$ modulo $\ell^nR_\ell$. Write $\ell^n\phi=a+\ell^nc$ with $c\in R_\ell$. Then $aT_\ell(E)\subseteq\ell^nT_\ell(E)$, so the divisibility statement gives $a/\ell^n\in R$. It follows that $\phi=a/\ell^n+c\in R_\ell$. Thus the [CM Tate module stabilizer](../../../../../cm-tate-module-stabilizer.md) is

$$
\boxed{\{\phi\in K_\ell:\phi T_\ell(E)\subseteq T_\ell(E)\}=R_\ell.}
$$

This does not presume freeness of the integral [Tate module](../../../../../tate-module.md) over a nonmaximal order.

For **(iii)**, every element of $R$ is defined over $k$, so the [Galois representation](../../../../../galois-representation.md) commutes with $R$ and therefore with $K_\ell$. By (i), its action on $V_\ell(E)$ is multiplication by an element of $K_\ell^\times$. The action and its inverse preserve $T_\ell(E)$; by (ii), this scalar and its inverse belong to $R_\ell$. Hence

$$
\boxed{\rho_\ell(G_k)\subseteq R_\ell^\times,\quad\text{so the image is abelian}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
