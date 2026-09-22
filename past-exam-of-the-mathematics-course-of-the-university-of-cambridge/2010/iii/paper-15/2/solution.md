<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A smooth rank-$r$ [vector bundle](../../../../../vector-bundle.md) over a [smooth manifold](../../../../../smooth-manifold.md) $M$ consists of a smooth total space $E$, a smooth projection $\pi:E\to M$, and an $r$-dimensional real [vector space](../../../../../vector-space-split.md) structure on each fibre $E_p=\pi^{-1}(p)$. Each point has a neighborhood $U$ with a [vector bundle trivialization](../../../../../vector-bundle-trivialization.md)

$$
\tau_U:\pi^{-1}(U)\xrightarrow{\sim}U\times\mathbb R^r
$$

that is a [diffeomorphism](../../../../../diffeomorphism.md), commutes with projection to $U$, and is a [linear isomorphism](../../../../../linear-isomorphism.md) on every fibre. The overlap maps have the form $(p,v)\mapsto(p,h(p)v)$ with $h:U\cap V\to GL_r(\mathbb R)$ smooth. For a complex [vector bundle](../../../../../vector-bundle.md), replace $\mathbb R$ by $\mathbb C$ and require complex-linear fibre maps.

A [connection on a vector bundle](../../../../../connection-vector-bundle.md) is an $\mathbb R$-linear map

$$
\nabla:\Gamma(E)\longrightarrow\Omega^1(M;E),\qquad
\nabla(fs)=df\otimes s+f\nabla s,
$$

where $\Gamma(E)$ is the [module of smooth sections](../../../../../module-of-smooth-sections.md), $\Omega^1(M;E)$ consists of [vector-bundle-valued differential forms](../../../../../vector-bundle-valued-differential-form.md) of degree one, and $f$ is a [smooth function](../../../../../smooth-function.md). Equivalently, evaluating on a [vector field](../../../../../vector-field.md) $X$ gives operators $\nabla_X$ with $\nabla_{fX}s=f\nabla_Xs$ and $\nabla_X(fs)=X(f)s+f\nabla_Xs$. A [connection on a vector bundle](../../../../../connection-vector-bundle.md) is local: its value at a point depends on the germ of the [section of a vector bundle](../../../../../section-of-a-vector-bundle.md), so the same definition applies to local sections.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 15](../../paper-15-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
