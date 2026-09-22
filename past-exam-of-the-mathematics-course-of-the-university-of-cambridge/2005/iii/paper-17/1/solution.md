<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $\mathcal I\subseteq\mathcal O_X$ be the [ideal sheaf](../../../../../ideal-sheaf-of-a-closed-subscheme.md) of $Y$. The [formal completion of a scheme](../../../../../formal-completion-of-a-scheme.md) along $Y$ has underlying topological space $|Y|$ and topological structure sheaf

$$
\boxed{X_{/Y}=\left(|Y|,\ \varprojlim_{n\geq0}(\mathcal O_X/\mathcal I^{n+1})|_{|Y|}\right).}
$$

The topology is the [adic topology](../../../../../adic-topology.md) given by the kernels of the projections to the successive [infinitesimal neighbourhoods](../../../../../infinitesimal-neighbourhood-of-a-closed-subscheme.md) $X_n=(|Y|,\mathcal O_X/\mathcal I^{n+1})$. In the locally [Noetherian scheme](../../../../../noetherian-scheme.md) setting of these examples this is a [formal scheme](../../../../../formal-scheme.md). On a Noetherian [affine scheme](../../../../../affine-scheme.md), with $Y=V(I)\subseteq\operatorname{Spec}A$, it is the [formal spectrum](../../../../../formal-spectrum.md) $\operatorname{Spf}\widehat A$, where $\widehat A=\varprojlim_nA/I^{n+1}$. Thus the completion retains all orders of infinitesimal information normal to $Y$.

Here $Z=D(t)=\operatorname{Spec}k[q,t,t^{-1}]$ is an [open subscheme](../../../../../open-subscheme.md) of $X$. The relevant affine completions are

$$
X_{/(q=0)}=\operatorname{Spf}\bigl(k[t][[q]]\bigr),\qquad
Z_{/(q=0)}=\operatorname{Spf}\bigl(k[t,t^{-1}][[q]]\bigr),
$$

with the $q$-adic topology. The complement of $t=0$ in the first [formal scheme](../../../../../formal-scheme.md) is its formal open $D(t)$. The sections on this open are the [completed localization of an adic ring](../../../../../completed-localization-of-an-adic-ring.md):

$$
\begin{aligned}
\Gamma(D(t),\mathcal O_{X_{/(q=0)}})
&=\varprojlim_{n\geq0}\bigl(k[t,q]/(q^{n+1})\bigr)[t^{-1}]\\
&=\varprojlim_{n\geq0}k[t,t^{-1},q]/(q^{n+1})
=k[t,t^{-1}][[q]].
\end{aligned}
$$

The same calculation on every smaller [principal open subset](../../../../../principal-open-subscheme.md) identifies the structure sheaves, not just their global sections. Equivalently, every [infinitesimal neighbourhood](../../../../../infinitesimal-neighbourhood-of-a-closed-subscheme.md) of $Z\cap(q=0)$ is precisely the restriction to $D(t)$ of the corresponding neighbourhood in $X$. By [formal completion commutes with restriction to an open subscheme](../../../../../formal-completion-commutes-with-restriction-to-an-open-subscheme.md),

$$
\boxed{Z_{/(q=0)}\ \cong\ X_{/(q=0)}\setminus(t=0).}
$$

The [isomorphism](../../../../../isomorphism.md) is canonical and respects the morphisms to $\operatorname{Spf}k[[q]]$.

It would give the wrong answer to replace the formal-open structure sheaf by the ordinary [localization of a ring](../../../../../localization-of-a-ring.md) $k[t][[q]][t^{-1}]$. That [ring](../../../../../ring.md) has a uniform bound on the negative powers of $t$ across the coefficients of any one element, whereas

$$
\sum_{n\geq0}q^nt^{-n}\ \in\ k[t,t^{-1}][[q]]
$$

has no such bound. This difference between ordinary and completed localization does not obstruct the [isomorphism](../../../../../isomorphism.md) of [formal schemes](../../../../../formal-scheme.md); it explains why the completed localization is essential.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
