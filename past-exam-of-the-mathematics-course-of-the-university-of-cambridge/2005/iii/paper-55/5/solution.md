<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Set $x=T+\bar T>0$, the domain in which the [Kähler potential](../../../../../kahler-potential.md) is defined, and use Planck units. The nonzero entries of the [Kähler metric](../../../../../kahler-metric.md) and its inverse are

$$
K_{T\bar T}=\frac3{x^2},\qquad K_{C\bar C}=1,
\qquad K^{T\bar T}=\frac{x^2}{3},\qquad K^{C\bar C}=1.
$$

The [Kähler covariant derivatives of a superpotential](../../../../../kahler-covariant-derivative-of-a-superpotential.md) are

$$
D_TW=-\frac3x(C^3+B),\qquad
D_CW=3C^2+\bar C(C^3+B).
$$

Denote $W=C^3+B$ and $S=3C^2+\bar C W$. The [supergravity F-term potential](../../../../../supergravity-f-term-potential.md) is

$$
V=e^K\left(K^{T\bar T}|D_TW|^2+|D_CW|^2-3|W|^2\right).
$$

Here the $T$ contribution is exactly $3|W|^2$, cancelling the negative term. This is the [no-scale supergravity](../../../../../no-scale-supergravity.md) identity, giving

$$
\boxed{V(T,C)=\frac{e^{|C|^2}}{x^3}\left|3C^2+\bar C(C^3+B)\right|^2\geq0.}
$$

The cancellation is important: replacing the covariant derivatives by ordinary derivatives would miss both the matter dependence and the possibility of zero [vacuum energy](../../../../../vacuum-energy.md) with [supersymmetry breaking](../../../../../supersymmetry-breaking.md).

In the convention $F^i=-e^{K/2}K^{i\bar j}\overline{D_jW}$, the chiral [supergravity auxiliary fields](../../../../../supergravity-auxiliary-field.md) are

$$
\boxed{F^T=e^{K/2}x\overline W
=\frac{e^{|C|^2/2}}{\sqrt x}(\bar C^3+\bar B),}
$$



$$
\boxed{F^C=-e^{K/2}\overline S
=-\frac{e^{|C|^2/2}}{x^{3/2}}
\left[3\bar C^2+C(\bar C^3+\bar B)\right].}
$$

An overall auxiliary phase or sign convention does not change their vanishing conditions. These are upper-index fields, including the inverse [Kähler metric](../../../../../kahler-metric.md), rather than just the covariant derivatives.

Since $V$ is nonnegative and vanishes at $C=0$, its minimum energy is

$$
\boxed{V_{\min}=0.}
$$

There are additional minima that should not be discarded by examining only real $C$. For $C=\rho e^{i\alpha}\ne0$, the condition $S=0$ becomes

$$
B=-\rho(3+\rho^2)e^{3i\alpha}.
$$

If $B\ne0$, the magnitude equation

$$
\rho^3+3\rho=|B|
$$

has exactly one positive root: its left side is strictly increasing from zero to infinity. There are three phases, differing by $2\pi/3$, determined by $e^{3i\alpha}=-B/|B|$. Thus for nonzero $B$ the finite zero-energy matter vacua consist of $C=0$ and these three nonzero phase-related values, each with arbitrary $T$ in the allowed half-plane. At a nonzero matter vacuum,

$$
W=C^3+B=-3\rho e^{3i\alpha}\ne0.
$$

At $C=0$, $W=B$.

For $B\ne0$, every such minimum has $F^C=0$ but $F^T\ne0$, so **supersymmetry is spontaneously broken despite zero vacuum energy**. Indeed no finite point anywhere is fully supersymmetric: $D_TW=0$ would force $W=0$, after which $D_CW=3C^2=0$ forces $C=0$ and then $B=0$. This proves breaking for the specified nonzero-constant case without relying just on the positivity of the potential.

**For the allowed exceptional value (B=0), the requested breaking statement is false.** Then $S=C^2(3+|C|^2)$ vanishes only at $C=0$, where $W=F^T=F^C=0$. Every finite allowed $T$ gives an unbroken [supersymmetric vacuum](../../../../../supersymmetric-vacuum.md) with zero energy. This is an explicit counterexample to unqualified breaking for an arbitrary complex $B$.

Both real components of $T$ are [flat directions of a scalar potential](../../../../../flat-direction-of-a-scalar-potential.md) along every minimum: the imaginary component never appears in $V$, and when $S=0$ the entire $x$ dependence is multiplied by zero. The matter vacua are isolated in the $C$ plane; there is no continuous matter vacuum direction. At $B=0$ the potential begins quartically in $C$, so zero quadratic mass is not a flat vacuum manifold. Away from $S=0$, the real $T$ direction instead has $V\propto x^{-3}$ and a decompactification-type runaway towards zero as $x\to\infty$, not a further finite positive-energy minimum.

The [gravitino mass from a superpotential](../../../../../gravitino-mass-from-a-superpotential.md) is

$$
\boxed{m_{3/2}=e^{K/2}|W|
=\frac{e^{|C|^2/2}|C^3+B|}{x^{3/2}}.}
$$

At the $C=0$ branch it is $|B|/x^{3/2}$; at each nonzero branch it is $3\rho e^{\rho^2/2}/x^{3/2}$. Its value is not fixed because the $T$ modulus is flat. For $B=0$ it vanishes at the supersymmetric minimum. For nonzero $B$, the [super-Higgs mechanism](../../../../../super-higgs-mechanism.md) absorbs the [Goldstino](../../../../../goldstino.md) associated with $F^T$ into the massive [gravitino](../../../../../gravitino.md). The zero-energy relation is explicitly satisfied:

$$
K_{T\bar T}|F^T|^2=3e^K|W|^2=3m_{3/2}^2,
$$

which balances the auxiliary contribution against the gravitational negative term.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
