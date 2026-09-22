<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Fix an explicit stationary-grid convention. For [subdivision arity](../../../../../subdivision-arity.md) $m>1$, write the univariate rule as

$$
p_i^{\ell+1}=\sum_jS_{ij}p_j^\ell,\qquad S_{ij}=a_{i-mj}.
$$

A column of the [subdivision matrix](../../../../../subdivision-matrix.md) is one translated [subdivision mask](../../../../../subdivision-mask.md); the next column is translated by $m$ fine-grid rows. Thus **the column displacement is the arity**. If $a_k$ is active from $k=\alpha$ to $k=\beta$, the [subdivision mask width](../../../../../subdivision-mask-width.md) is $w=\beta-\alpha+1$ fine-grid positions, after removing zero padding. Equivalently the mask span is $\beta-\alpha$ fine intervals. This is different from counting old [control points](../../../../../control-point.md) in a row stencil: that count measures how many controls influence one newly created point. Stating the convention avoids confusing these two widths.

For a convergent [subdivision curve](../../../../../subdivision-curve.md) scheme, its support is the influence region of one original [control point](../../../../../control-point.md), equivalently the [support of a function](../../../../../support.md) of the basic limit $\phi$ obtained from data $p_j=\delta_{j0}$. Translation gives the representation $P(t)=\sum_jp_j\phi(t-j)$. Descendant indices of index zero have parameter positions

$$
\frac{k_1}{m}+\frac{k_2}{m^2}+\cdots+\frac{k_\ell}{m^\ell},\qquad k_r\in[\alpha,\beta].
$$

Thus the limiting support enclosure is $[\alpha/(m-1),\beta/(m-1)]$, as in the [support of a stationary subdivision scheme](../../../../../support-of-a-stationary-subdivision-scheme.md). Endpoint activity gives equality for the ordinary positive convergent masks under discussion.

The [functional precision set of a subdivision scheme](../../../../../functional-precision-set-of-a-subdivision-scheme.md) consists of functions exactly recovered from their uniformly sampled data using the scheme's consistent parameter placement. Polynomial precision records the exactly reproduced [polynomial](../../../../../polynomial-split.md) space. Sampling-grid spacing and origin must be specified; the usual arbitrary-grid precision requirement uses every spacing and shift, rather than merely membership in the fixed-grid reconstruction space.

Center the given mask at indices $-1,0,1$. Its [binary linear interpolatory subdivision](../../../../../binary-linear-interpolatory-subdivision.md) rule is

$$
p'_{2j}=p_j,\qquad p'_{2j+1}=\tfrac12(p_j+p_{j+1}).
$$

Each new [control point](../../../../../control-point.md) is either an old point or an edge midpoint. Hence every refined [control polygon](../../../../../control-polygon.md) is the same [curve](../../../../../curve.md) with extra vertices. Starting from scalar impulse data, the limit is explicitly

$$
\phi(t)=\max(1-|t|,0),\qquad\boxed{\operatorname{supp}\phi=[-1,1].}
$$

The mask width is three positions, its mask span is two, its largest row stencil uses two old [control points](../../../../../control-point.md), and its [subdivision arity](../../../../../subdivision-arity.md) is two. Translating the mask indexing to $0,1,2$ translates the basic support to $[0,2]$; the support width remains two original grid intervals.

On $[j,j+1]$, reconstruction is $(j+1-t)p_j+(t-j)p_{j+1}$. Constant and affine samples are therefore recovered exactly. A non-affine [polynomial](../../../../../polynomial-split.md) cannot agree with a linear expression on a whole open interval. Thus its polynomial [functional precision set of a subdivision scheme](../../../../../functional-precision-set-of-a-subdivision-scheme.md) is

$$
\boxed{\mathcal P=\operatorname{span}\{1,t\}.}
$$

For continuous functions reproduced at every translated sampling grid, the same conclusion holds: agreement with all chord interpolants forces the affine interpolation identity, hence affinity. At one fixed grid, the larger exactly representable class is the space of [linear splines](../../../../../linear-spline.md) with those [spline knots](../../../../../spline-knot.md); this is not a higher polynomial precision claim.

For arbitrary data, the one-sided [derivatives](../../../../../derivative.md) at $j$ are $p_j-p_{j-1}$ and $p_{j+1}-p_j$. They need not coincide. Therefore **the generic limit is $C^0$, not $C^1$**. Its first [derivative](../../../../../derivative.md) is piecewise constant; exceptional affine data, or individual matching neighboring slopes, can be smoother. This conclusion follows directly from the limit formula, not just from a heuristic mask-width test.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
