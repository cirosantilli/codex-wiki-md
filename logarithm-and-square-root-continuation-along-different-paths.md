# Logarithm and square-root continuation along different paths

↑ **Parent:** [Monodromy theorem](monodromy-theorem.md)

Start at $a=1$ with [complex logarithm](complex-logarithm.md) [germ of a holomorphic function](germ-of-a-holomorphic-function.md) $L(1)=0$ and [holomorphic square root](holomorphic-square-root.md) [germ of a holomorphic function](germ-of-a-holomorphic-function.md) $S(1)=1$. On the [punctured plane](punctured-complex-plane.md) $D=\mathbb C\setminus\{0\}$, both admit [analytic continuation](analytic-continuation.md) along every [path](continuous-path.md). To construct it locally, for any $c\ne0$ choose a small [open disc](open-disc.md) avoiding $0$, select a [holomorphic logarithm](holomorphic-logarithm.md) there, and select its additive multiple of $2\pi i$ to agree with the arriving [germ of a holomorphic function](germ-of-a-holomorphic-function.md); exponentiating half this logarithm supplies the arriving [holomorphic square root](holomorphic-square-root.md). A finite chain of these [open discs](open-disc.md) follows any given [path](continuous-path.md).

Compare two [paths](continuous-path.md) from $1$ to $i$, parametrized by $0\le t\le1$:

$$
\gamma_A(t)=e^{i\pi t/2},\qquad \gamma_B(t)=e^{-3i\pi t/2}.
$$

The first follows a counterclockwise quarter-circle; the second follows a clockwise three-quarter-circle. Following $\gamma_A$ and then [path reversal](path-reversal.md) of $\gamma_B$ makes one positive turn about $0$. Its [winding number](winding-number.md) is $1$, so the two [paths](continuous-path.md) cannot be [homotopic](homotopy-split.md) with endpoints fixed in the [punctured plane](punctured-complex-plane.md).

<a id="image-two-paths-from-1-to-i-enclose-the-puncture-while-a-negative-real-axis-cut-excludes-the-clockwise-route-and-permits-a-deformation-between-the-remaining-routes"></a>
![](monodromy-paths-and-slit-domain.png)

**[Figure 4](#image-two-paths-from-1-to-i-enclose-the-puncture-while-a-negative-real-axis-cut-excludes-the-clockwise-route-and-permits-a-deformation-between-the-remaining-routes). Two paths from 1 to i enclose the puncture, while a negative-real-axis cut excludes the clockwise route and permits a deformation between the remaining routes**.

The continued values along the chosen [paths](continuous-path.md) are

$$
L_A(t)=\frac{\pi i t}{2},\qquad L_B(t)=-\frac{3\pi i t}{2},\qquad S_A(t)=e^{i\pi t/4},\qquad S_B(t)=e^{-3i\pi t/4}.
$$

At their common endpoint,

$$
L_A(1)=\frac{\pi i}{2},\quad L_B(1)=-\frac{3\pi i}{2},\quad L_A(1)-L_B(1)=2\pi i,
\qquad S_A(1)=\frac{1+i}{\sqrt2},\quad S_B(1)=-\frac{1+i}{\sqrt2}.
$$

Both [complex logarithm](complex-logarithm.md) values exponentiate to $i$, and both [holomorphic square root](holomorphic-square-root.md) values square to $i$. These give different terminal [germ of a holomorphic function](germ-of-a-holomorphic-function.md) representatives, consistently obtained from the same starting [germ of a holomorphic function](germ-of-a-holomorphic-function.md). The [monodromy theorem](monodromy-theorem.md) applies, but does not equate these two non-[homotopic](homotopy-split.md) [paths](continuous-path.md).

<a id="image-tracking-continuation-from-1-to-i-along-a-quarter-circle-and-a-clockwise-three-quarter-circle-gives-logarithms-separated-by-2-pi-i-and-opposite-square-roots"></a>
![](monodromy-logarithm-square-root-path-tracking.png)

**[Figure 5](#image-tracking-continuation-from-1-to-i-along-a-quarter-circle-and-a-clockwise-three-quarter-circle-gives-logarithms-separated-by-2-pi-i-and-opposite-square-roots). Tracking continuation from 1 to i along a quarter-circle and a clockwise three-quarter-circle gives logarithms separated by 2 pi i and opposite square roots**.

The closed [path](continuous-path.md) $\lambda(t)=e^{2\pi it}$ instead returns to $1$, with continued values $L_\lambda(t)=2\pi it$ and $S_\lambda(t)=e^{\pi it}$. One counterclockwise turn changes the [complex logarithm](complex-logarithm.md) by $2\pi i$ and flips the [holomorphic square root](holomorphic-square-root.md) from $1$ to $-1$. Hence neither initial [germ of a holomorphic function](germ-of-a-holomorphic-function.md) can come from a global [holomorphic logarithm](holomorphic-logarithm.md) or a global [holomorphic square root](holomorphic-square-root.md) of $z$ on the [punctured plane](punctured-complex-plane.md). Repeating a [loop](loop-topology.md) of [winding number](winding-number.md) $n$ gives the changes $2\pi in$ and $(-1)^n$. [Rosales, Branch Points and Branch Cuts, section 1, printed pp. 3–8, and Example 2.4, printed p. 15](branch-points-and-branch-cuts-by-rodolfo-r-rosales.md)

Now restrict to the slit [domain](domain-mathematical-analysis.md) $D_{\mathrm{slit}}=\mathbb C\setminus(-\infty,0]$. The [principal logarithm](principal-complex-logarithm.md) and $\exp(\operatorname{Log}z/2)$ realize the same initial [germ of a holomorphic function](germ-of-a-holomorphic-function.md) for each expression globally. To see that this is a [simply connected domain](simply-connected-domain.md), [polar form](polar-form-of-a-complex-number.md) identifies this [domain](domain-mathematical-analysis.md) with $(0,\infty)\times(-\pi,\pi)$, a [convex set](convex-set-split.md); every [loop](loop-topology.md) contracts there. The [simply connected corollary of the monodromy theorem](simply-connected-corollary-of-the-monodromy-theorem.md) now forces equality along every pair of [paths](continuous-path.md) with matching endpoints. In particular, $\gamma_A$ and the segment $\sigma(t)=1-t+it$ both give $L(i)=\pi i/2$ and $S(i)=(1+i)/\sqrt2$. The explicit [homotopy](homotopy-split.md) $H(s,t)=(1-s)\gamma_A(t)+s\sigma(t)$ stays in the closed first quadrant away from $0$, hence in $D_{\mathrm{slit}}$.

The other route $\gamma_B$ crosses the removed ray at $t=2/3$ and is no longer admissible. In the [punctured plane](punctured-complex-plane.md), that crossing is locally regular: [analytic continuation](analytic-continuation.md) passes through $-1$ smoothly, although evaluating the [principal logarithm](principal-complex-logarithm.md) would reset its [argument](argument-complex-analysis.md). The [branch cut](branch-cut.md) changes the allowed [domain](domain-mathematical-analysis.md); it does not create additional [branch points](branch-point.md) or [poles](pole.md). That distinction is the beauty of the obstruction: perfectly compatible local [holomorphic functions](holomorphic-function-split.md) can fail to make a global choice solely because of the allowed [based loops](based-loop.md). The [branches of a multivalued function](branch-of-a-multivalued-function.md) article develops how moving the [branch cut](branch-cut.md) changes the selected values.

## ↑ Ancestors (8)

1. [Monodromy theorem](monodromy-theorem.md)
2. [Analytic continuation](analytic-continuation.md)
3. [Holomorphic function](holomorphic-function-split.md)
4. [Complex analysis](complex-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Monodromy group of a covering](monodromy-group-of-a-covering.md)
