<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Choose a small skeleton $\mathcal F$ of the [finite spectra](../../../../../finite-spectrum.md), including every integer suspension. There is such a set of representatives: a finite list of stable cells and their attaching maps specifies a finite cell model, and the possible attaching maps form sets. For every $F\in\mathcal F$ and every stable map $v:F\to D$, take one copy of $F$ and form

$$
X=\bigvee_{(F,v)}F.
$$

Define the evaluation map $e:X\to D$ by taking its restriction to the $(F,v)$ summand to be $v$. Complete it to the [cofiber sequence of spectra](../../../../../cofiber-sequence-of-spectra.md)

$$
X\xrightarrow{e}D\xrightarrow{p}E\longrightarrow\Sigma X.
$$

This is the [universal evaluation phantom map](../../../../../universal-evaluation-phantom-map.md) construction.

First, $p$ is nonzero. If $p=0$, applying $[D,-]_{\mathrm{st}}$ to the [cofiber sequence of spectra](../../../../../cofiber-sequence-of-spectra.md) gives the exact portion

$$
[D,X]_{\mathrm{st}}\xrightarrow{e_*}[D,D]_{\mathrm{st}}\xrightarrow{p_*}[D,E]_{\mathrm{st}}.
$$

Since $p_*(1_D)=p=0$, exactness supplies $s:D\to X$ with $es=1_D$. Thus $D$ is a [retract](../../../../../retract.md) of $X$. This is also a wedge summand: complete $s$ to a [cofiber sequence of spectra](../../../../../cofiber-sequence-of-spectra.md) $D\to X\to C'\to\Sigma D$. The left inverse $e$ makes this triangle split, giving $X\cong D\vee C'$ in the [stable homotopy category](../../../../../stable-homotopy-category.md). One can see the splitting directly from exactness: the connecting map is zero because $e$ extends $1_D$ across $s$, and consequently the quotient map $X\to C'$ admits a section. This contradicts the assumption on $D$. Hence $p\ne0$.

For any [finite spectrum](../../../../../finite-spectrum.md) $F$ and any $v:F\to D$, its chosen representative has a summand inclusion $\iota_v:F\to X$ with $e\iota_v=v$, after transferring along the representative isomorphism. Consecutive maps of a [cofiber sequence of spectra](../../../../../cofiber-sequence-of-spectra.md) compose to zero, so

$$
pv=pe\iota_v=0.
$$

Thus $p$ is a [phantom map of spectra](../../../../../phantom-map-of-spectra.md). To establish the requested conclusion on all spaces, rather than just coefficient groups, let $K$ first be a finite based [CW complex](../../../../../cw-complex.md). Put $A=\Sigma^\infty K$. The [Spanier-Whitehead dual](../../../../../spanier-whitehead-dual.md) $A^\vee=F(A,\mathbb S)$ is a [finite spectrum](../../../../../finite-spectrum.md). The evaluation and coevaluation adjunction of [Spanier-Whitehead duality](../../../../../spanier-whitehead-duality.md) identifies

$$
\widetilde D_k(K)=\pi_k(D\wedge A)\cong[\Sigma^kA^\vee,D]_{\mathrm{st}}.
$$

Under this identification $p_*$ is postcomposition with $p$. Its source is a [finite spectrum](../../../../../finite-spectrum.md), including when $k$ is negative, so the calculation $pv=0$ proves that $p_*$ is zero on $\widetilde D_k(K)$ for every $k$.

Now let $Y$ be an arbitrary based [CW complex](../../../../../cw-complex.md). It is the filtered union, or filtered [homotopy colimit of spaces](../../../../../homotopy-colimit-of-spaces.md), of its finite based subcomplexes $K$. The [suspension spectrum](../../../../../suspension-spectrum.md) functor and [smash product of spectra](../../../../../smash-product-of-spectra.md) preserve that homotopy colimit. The shifted [sphere spectrum](../../../../../sphere-spectrum.md) is compact, so taking [stable homotopy groups](../../../../../stable-homotopy-group.md) gives

$$
\widetilde D_k(Y)=\operatorname*{colim}_{K\subset Y\ \mathrm{finite}}\widetilde D_k(K),\qquad\widetilde E_k(Y)=\operatorname*{colim}_{K\subset Y\ \mathrm{finite}}\widetilde E_k(K).
$$

Every element of the first group therefore comes from a finite $K$, where $p_*$ has just been proved zero. Consequently $p_*$ is zero on $Y$ as well. A based [CW complex](../../../../../cw-complex.md) replacement extends the conclusion to arbitrary based spaces in the homotopy category. We have constructed

$$
\boxed{p:D\longrightarrow E,\qquad p\ne0\text{ stably},\qquad p_*:\widetilde D_*(Y)\longrightarrow\widetilde E_*(Y)\text{ is zero for every }Y.}
$$

This uses continuity of [represented homology theory](../../../../../represented-homology-theory.md), not a continuity assertion for [represented cohomology theory](../../../../../represented-cohomology-theory.md); the latter need not hold.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
