<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $S=\Phi_0$, $u=\Phi_+$, $v=\Phi_-$, $M=M_p$, $P=uv-\zeta$, $x=|S|^2/M^2$ and $q=|u|^2+|v|^2$. Assume $g\ne0$ and, initially, $\zeta\ne0$. The [supergravity F-term potential](../../../../../supergravity-f-term-potential.md) is

$$
V_F=e^{K/M^2}\left(K^{i\bar j}D_iW\overline{D_jW}-\frac{3|W|^2}{M^2}\right),\qquad D_iW=W_i+\frac{K_iW}{M^2}.
$$

The canonical [Kähler potential](../../../../../kahler-potential.md) gives the identity [Kähler metric](../../../../../kahler-metric.md). The three [Kähler covariant derivatives of a superpotential](../../../../../kahler-covariant-derivative-of-a-superpotential.md) are

$$
D_SW=gP(1+x),\qquad D_uW=gS\left(v+\frac{\bar uP}{M^2}\right),\qquad D_vW=gS\left(u+\frac{\bar vP}{M^2}\right).
$$

Substituting, including the negative term rather than treating the potential as just a sum of squares, gives the exact answer

$$
\boxed{V_F=|g|^2e^{x+q/M^2}\left[(1-x+x^2)|uv-\zeta|^2+|S|^2\left(\left|v+\frac{\bar u(uv-\zeta)}{M^2}\right|^2+\left|u+\frac{\bar v(uv-\zeta)}{M^2}\right|^2\right)\right].}
$$

Here $(1+x)^2-3x=1-x+x^2$ explains the first coefficient. It is strictly positive for real $x$, since $1-x+x^2=(x-1/2)^2+3/4$. Thus this model's [scalar potential](../../../../../scalar-potential.md) is nonnegative everywhere.

In the stated limit $q/M^2\ll1$, the exponential can be replaced by $e^x[1+O(q/M^2)]$. The other displayed terms retain the effects of the [Kähler covariant derivatives of a superpotential](../../../../../kahler-covariant-derivative-of-a-superpotential.md). Small waterfall fields alone do not justify discarding $\zeta/M^2$ in those derivatives, or expanding in $x$. If also $|\zeta|/M^2\ll1$ and $x\ll1$, the leading result reduces to the global [F-term scalar potential](../../../../../f-term-scalar-potential.md)

$$
V_{\mathrm{global}}=|g|^2\left(|uv-\zeta|^2+|S|^2q\right).
$$

No gauge sector or gauge coupling is supplied, so there is no specified [D-term](../../../../../d-term.md) contribution to add.

The [supersymmetric vacuum manifold of a bilinear hybrid superpotential](../../../../../supersymmetric-vacuum-manifold-of-a-bilinear-hybrid-superpotential.md) is

$$
\boxed{S=0,\qquad uv=\zeta,\qquad V_F=0.}
$$

Indeed $W=0$ and all three [Kähler covariant derivatives of a superpotential](../../../../../kahler-covariant-derivative-of-a-superpotential.md) vanish there, so all [supergravity auxiliary fields](../../../../../supergravity-auxiliary-field.md) vanish and [supersymmetry](../../../../../supersymmetry-split.md) is unbroken. The nonnegative [scalar potential](../../../../../scalar-potential.md) makes this a global minimum. Conversely zero potential requires $uv=\zeta$, and then $|S|^2q=0$; for $\zeta\ne0$ this forces $S=0$. With just the supplied fields this is a complex [vacuum manifold](../../../../../vacuum-manifold.md) before imposing any gauge quotient: the product is fixed but the ratio of $u$ and $v$ is not. More precisely, it is an F-flat vacuum manifold whether or not a gauge symmetry is specified. If one additionally gauges opposite charges, [D-flatness](../../../../../d-flatness.md) typically imposes $|u|=|v|$, giving $|u|=|v|=\sqrt{|\zeta|}$ up to phases and gauge equivalence; that is an extra assumption, not a consequence of $K$ and $W$ alone.

The other familiar branch of [F-term hybrid inflation](../../../../../f-term-hybrid-inflation.md) has $u=v=0$. Its nonzero derivative $D_SW=-g\zeta(1+x)$ establishes [supersymmetry breaking](../../../../../supersymmetry-breaking.md), and its exact [scalar potential](../../../../../scalar-potential.md) is

$$
\boxed{V_0(S)=|g\zeta|^2e^x(1-x+x^2).}
$$

The [canonical-Kähler correction to an F-term hybrid valley](../../../../../canonical-kahler-correction-to-an-f-term-hybrid-valley.md) begins as

$$
V_0=|g\zeta|^2\left(1+\frac{x^2}{2}+O(x^3)\right).
$$

In particular the [inflaton](../../../../../inflaton.md) quadratic mass cancels at this order; the first lift of the global flat valley is quartic in $|S|$.

To identify when this branch is a transverse minimum, rephase the waterfall fields so that $\zeta$ is real positive. To quadratic order in $u,v$, the global [scalar potential](../../../../../scalar-potential.md) is

$$
|g\zeta|^2+|g|^2\left[|S|^2(|u|^2+|v|^2)-|\zeta|(uv+\bar u\bar v)\right].
$$

The normalized combinations $(u\pm\bar v)/\sqrt2$ diagonalize this quadratic form, with

$$
\boxed{m_\pm^2=|g|^2(|S|^2\pm|\zeta|)\quad\text{in the global approximation}.}
$$

Thus $|S|^2>|\zeta|$ gives a valley of transverse minima, while below the threshold the negative [eigenvalue](../../../../../eigenvalue.md) produces the [waterfall instability in F-term hybrid inflation](../../../../../waterfall-instability-in-f-term-hybrid-inflation.md).

The exact supergravity correction to this stability test is also available without taking $x$ small. Put $b=|\zeta|/M^2$. Expansion of the exact [supergravity F-term potential](../../../../../supergravity-f-term-potential.md) about $u=v=0$ gives equal diagonal coefficients $|g|^2M^2e^x[x+b^2(1+x^2)]$ and off-diagonal magnitude $|g|^2M^2e^xb(1+x+x^2)$. Hence

$$
m_\pm^2=|g|^2M^2e^x\left[x+b^2(1+x^2)\pm b(1+x+x^2)\right].
$$

For the usual sub-Planckian symmetry-breaking scale $0<b\ll1$, the lower [eigenvalue](../../../../../eigenvalue.md) is $|g|^2M^2e^x(1-b)[x-b(1+x^2)]$. It is positive for the familiar sub-Planckian valley $b\ll x\ll1$, and changes sign near $x=b$.

**The printed assertion of two full minima requires qualification.** The broken branch is a transverse inflationary valley, not generally a second stationary minimum of the complete supergravity potential. In fact

$$
\frac{dV_0}{dx}=|g\zeta|^2e^xx(1+x)>0\qquad(x>0).
$$

Its only stationary point in $S$ is the origin. For $0<|\zeta|<M^2$ that point has a negative waterfall [eigenvalue](../../../../../eigenvalue.md) $|g|^2(|\zeta|^2/M^2-|\zeta|)$. A direct counterexample is the path $S=0$, $u=v=a$ with real small $a$, after rephasing $\zeta>0$:

$$
V_F=|g|^2e^{2a^2/M^2}(a^2-\zeta)^2=|g|^2\zeta^2+2|g|^2\left(\frac{\zeta^2}{M^2}-\zeta\right)a^2+O(a^4).
$$

The negative quadratic coefficient proves it is not a minimum. No loop corrections or additional stabilizing interactions were specified that could create the requested second stationary vacuum. The mathematically supported interpretation is **a SUSY-breaking transverse valley and a zero-energy [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md) minimum manifold**. The limit on $u,v$ alone does not fix the parameter range $|\zeta|/M^2$; the familiar waterfall conclusion uses the sub-Planckian range just stated.

In the corresponding global theory the exponential prefactor, Kähler corrections to $D_iW$ and universal $-3|W|^2/M^2$ term are absent. Its $u=v=0$ valley has exactly constant tree-level energy $|g\zeta|^2$ for all $S$, whereas canonical [supergravity](../../../../../supergravity.md) lifts it by the quartic correction above. The [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md) $S=0$, $uv=\zeta$ and its zero energy persist in both descriptions. If $\zeta=0$, the origin and the $S$ axis instead have vanishing F-terms; the broken-valley interpretation does not apply.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
