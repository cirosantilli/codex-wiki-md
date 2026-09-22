<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

We first construct a genuinely compact [Besicovitch set](../../../../../besicovitch-set.md); a sequence of unrelated small-area sets would not suffice. The [compact Kakeya construction from small projections](../../../../../compact-kakeya-construction-from-small-projections.md) below gives the limiting [compact set](../../../../../compact-space.md) together with its segments.

Let $\mathcal X$ consist of nonempty [compact sets](../../../../../compact-space.md) $K\subset[0,1]\times\mathbb R$ whose horizontal projection is exactly $[0,1]$. With the [Hausdorff metric](../../../../../hausdorff-distance.md) this is a [complete metric space](../../../../../complete-metric-space.md). Indeed a Hausdorff-Cauchy sequence is eventually contained in one bounded closed rectangle and converges there to a nonempty [compact set](../../../../../compact-space.md); horizontal projection is Lipschitz for Hausdorff distance, so its value $[0,1]$ is preserved in the limit.

For $t\in[0,1]$ put $L_t(x,y)=y+tx$ and $m_t(K)=|L_t(K)|$. The [function](../../../../../function-split.md) $(K,t)\mapsto m_t(K)$ is [upper semicontinuous](../../../../../upper-semicontinuity.md). To verify this, cover the [compact set](../../../../../compact-space.md) $L_t(K)$ by finitely many open intervals with total length less than $m_t(K)+\varepsilon$. Joint continuity of the compact images in the [Hausdorff metric](../../../../../hausdorff-distance.md) puts every sufficiently nearby image inside the same cover. This proves the required upper bound, uniformly over a compact parameter interval when a strict bound holds throughout it.

Fix $q\in[0,1]$ and $\varepsilon>0$. The set

$$
U(q,\varepsilon)=\{K\in\mathcal X:\sup_{t\in[0,1],\,|t-q|\le\varepsilon}m_t(K)<2\varepsilon\}
$$

is open. It is also dense, by the following explicit finite approximation. Given $K$ and tolerance $h>0$, partition $[0,1]$ into $N$ equal subintervals and choose $(j/N,y_j)\in K$ at each left endpoint. Above that subinterval put the segment

$$
\{(x,y_j-q(x-j/N)):j/N\le x\le(j+1)/N\}.
$$

Each segment lies within $\sqrt{1+q^2}/N$ of its chosen point in $K$. Add a finite $h/2$-net of points of $K$ to their union, ensuring the reverse Hausdorff inclusion. For large $N$ the resulting [compact set](../../../../../compact-space.md) $K'$ belongs to $\mathcal X$ and has Hausdorff distance less than $h$ from $K$. The image of each segment under $L_t$ has length $|t-q|/N$, and the added points contribute zero length. Hence

$$
m_t(K')\le|t-q|\le\varepsilon\quad\text{if }|t-q|\le\varepsilon,
$$

so $K'\in U(q,\varepsilon)$.

Take a finite grid of $q$'s whose $\varepsilon$-neighborhoods cover $[0,1]$. The finite intersection of the open dense sets $U(q,\varepsilon)$ is dense and implies $\sup_{0\le t\le1}m_t(K)<2\varepsilon$. Thus

$$
V_\varepsilon=\{K:\sup_{0\le t\le1}m_t(K)<2\varepsilon\}
$$

is open and dense. The [Baire category theorem](../../../../../baire-category-theorem.md) gives a compact $K\in\bigcap_{r\ge1}V_{1/r}$, and therefore $m_t(K)=0$ for every $t\in[0,1]$.

Define

$$
B=\{(t,y+tx):(x,y)\in K,\ 0\le t\le1\}.
$$

This is the [continuous](../../../../../continuous-function.md) image of the [compact set](../../../../../compact-space.md) $K\times[0,1]$, hence compact. Its section at horizontal coordinate $t$ is $L_t(K)$, of measure zero. The [Fubini theorem](../../../../../fubini-s-theorem.md) gives $|B|=\int_0^1m_t(K)\,dt=0$. For every slope $x\in[0,1]$, horizontal surjectivity supplies $(x,y)\in K$, and $B$ contains the segment $(t,y+tx)$, $0\le t\le1$, of length $\sqrt{1+x^2}\ge1$. Four rotated copies, through angles $0,\pi/4,\pi/2,3\pi/4$, cover all unoriented directions. Their finite union $\mathcal B$ is compact, has area zero, and contains a unit subsegment in every direction:

$$
\boxed{|\mathcal B|=0,\qquad\mathcal B\text{ compact and containing all unit-segment directions}.}
$$

The point-line dual construction is the mechanism in [Körner's construction](https://www.impan.pl/en/publishing-house/journals-and-series/studia-mathematica/all/158/1/90428/besicovitch-via-baire); the density calculation above supplies the needed proof, rather than assuming that small-area sets automatically admit a suitable nested limit.

For the multiplier discussion, define $T_D$ by $\widehat{T_Dg}(\xi)=\mathbf1_{\{|\xi|\le1\}}\widehat g(\xi)$. The [Plancherel theorem](../../../../../plancherel-theorem.md) gives boundedness on $L^2$. We explain why a putative $L^p$ bound, $1<p<2$, would contradict Kakeya packing; [duality of Lp spaces](../../../../../duality-of-lp-spaces.md) then treats $p>2$.

First, such a bound would force the vector-valued inequality

$$
\left\|\left(\sum_j|P_{v_j}g_j|^2\right)^{1/2}\right\|_p
\le C_p\left\|\left(\sum_j|g_j|^2\right)^{1/2}\right\|_p
$$

for arbitrary directions $v_j$, where $P_v$ is the [half-plane Fourier projection](../../../../../half-plane-fourier-projection.md) onto the half-plane $\xi\cdot v<0$. To see the important curvature step, let $T_R$ project onto the radius-$R$ disk and modulate by $e^{iRv_j\cdot x}$. Its conjugated symbol is $\mathbf1_{\{|\xi+Rv_j|\le R\}}$, tending almost everywhere to $\mathbf1_{\{\xi\cdot v_j<0\}}$. Dilations give the same putative [norm](../../../../../norm.md) bound for every $R$. Apply this common operator to $\sum_j\epsilon_je^{iRv_j\cdot x}g_j$, average over independent random signs, and use the [Khintchine inequality](../../../../../khintchine-inequality.md). Letting $R\to\infty$ gives the displayed estimate by $L^2$ convergence and [Fatou lemma](../../../../../fatou-s-lemma.md), first for finitely many [smooth function](../../../../../smooth-function.md) [functions](../../../../../function-split.md) and then by approximation. The disk has a boundary normal in every direction; a fixed polygon does not.

The geometric input for this overview is the standard finite [Perron tree](../../../../../perron-tree.md) packing used in [Fefferman's original proof](https://web.ma.utexas.edu/users/tc/M393C-F10/SolutionsF10/Fefferman-BallMultiplierKakeya.pdf): for arbitrarily small $\eta>0$ one obtains long thin rectangles $R_j$ with $A=\sum_j|R_j|$ and $|\bigcup_jR_j|\le\eta A$, while fixed longitudinal translates $R'_j$ are pairwise disjoint. This is a quantitative finite arrangement, stronger than merely having a compact null set. The splitting/sliding procedure subdivides an angular triangle into narrow triangles and overlaps their bases; the extensions along their axes separate in reverse order. Its area estimate has the form $\alpha^{2m}+2(1-\alpha)$ relative to the original total triangle area: the merged central part shrinks by $\alpha^2$ at each generation, and the accumulated caps contribute at most $2(1-\alpha)$. Taking $\alpha$ close to one and then $m$ large makes the ratio arbitrarily small. Inscribed rectangular portions retain a fixed proportion of the total area. The reflected extensions explain why the translates can be disjoint even though the original rectangles overlap strongly.

Here is the analytic contradiction, with the relevant powers explicit. Take $g_j=\mathbf1_{R_j}$. In coordinates parallel and perpendicular to the long axis $v_j$, the [directional Hilbert transform](../../../../../directional-hilbert-transform.md) integrates only along that axis. If the longitudinal interval is $[0,\ell]$, then outside it

$$
H_{v_j}\mathbf1_{R_j}(s,r)=\frac1\pi\log\left|\frac{s}{s-\ell}\right|\mathbf1_{\text{transverse interval}}(r).
$$

On a fixed translate such as $s\in[5\ell,6\ell]$, this has magnitude at least $\pi^{-1}\log(6/5)$. Since $P_v=(I-iH_v)/2$ up to the harmless choice of half-plane sign, $|P_{v_j}g_j|\ge c_0>0$ on $R'_j$. Their disjointness gives a lower bound $c_0A^{1/p}$ for the vector-valued output [norm](../../../../../norm.md).

Writing $h=\sum_j\mathbf1_{R_j}$, [Hölder's inequality](../../../../../holder-s-inequality.md) for $p<2$ gives

$$
\int h^{p/2}\le|\bigcup_jR_j|^{1-p/2}\left(\int h\right)^{p/2},
\qquad\left\|h^{1/2}\right\|_p\le|\bigcup_jR_j|^{1/p-1/2}A^{1/2}.
$$

The putative vector-valued inequality would imply

$$
c_0\le C_p\left(\frac{|\bigcup_jR_j|}{A}\right)^{1/p-1/2}\le C_p\eta^{1/p-1/2},
$$

which is impossible as $\eta\downarrow0$. The disk multiplier is self-adjoint, so a bound for $p>2$ would give one for its conjugate exponent below two. Thus **the disk multiplier is bounded only at $p=2$** among $1<p<\infty$. This explains both the random-sign step and the precise geometric amplification; it is not an assertion that frequency rectangles by themselves produce a logarithmic [norm](../../../../../norm.md) blow-up.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [Section C](../section-c.md)
3. [Paper 82](../../paper-82-split.md)
4. [Iii](../../split.md)
5. [2012](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
