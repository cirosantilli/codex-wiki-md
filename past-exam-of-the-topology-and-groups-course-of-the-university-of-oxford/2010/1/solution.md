<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [homotopy](../../../homotopy-split.md) from $f_0:Y\to X$ to $f_1:Y\to X$ is a [continuous map](../../../continuous-map.md) $H:Y\times[0,1]\to X$ with $H(y,0)=f_0(y)$ and $H(y,1)=f_1(y)$ for every $y$. A [covering map](../../../covering-space.md) $p:\widetilde X\to X$ is a surjective [continuous map](../../../continuous-map.md) for which every $x\in X$ has an open neighborhood $U$ whose inverse image is a disjoint union of open sets, each mapped homeomorphically onto $U$. A [lift](../../../lift-force-split.md) of $f:Y\to X$ is a [continuous map](../../../continuous-map.md) $\widetilde f:Y\to\widetilde X$ satisfying $p\circ\widetilde f=f$.

The [path lifting theorem](../../../path-lifting-theorem.md) says that a [path](../../../continuous-path.md) $\gamma:[0,1]\to X$ and a point $\widetilde x_0\in p^{-1}(\gamma(0))$ determine a unique [path](../../../continuous-path.md) $\widetilde\gamma:[0,1]\to\widetilde X$ with $p\widetilde\gamma=\gamma$ and $\widetilde\gamma(0)=\widetilde x_0$.

On $S^1\setminus\{1\}$ there is a continuous branch $\operatorname{Arg}_{(0,2\pi)}$ of the [complex argument](../../../argument-complex-analysis.md), taking values in $(0,2\pi)$. If $f$ avoids $1$, set $\theta(z)=\operatorname{Arg}_{(0,2\pi)}f(z)$. Then the explicit [homotopy](../../../homotopy-split.md)

$$
\boxed{H(z,s)=\exp\big(i((1-s)\theta(z)+s\pi)\big)}
$$

starts at $f$ and ends at the constant map $-1$. It is continuous because the chosen argument branch is continuous on the whole image. More generally, a map omitting any $w\in S^1$ is [null-homotopic](../../../null-homotopic-map.md): apply the formula to $\overline w f$ and multiply the resulting [homotopy](../../../homotopy-split.md) by $w$.

For the based injective map, use the standard [covering map](../../../covering-space.md) $E(t)=e^{2\pi it}$. [Lift](../../../lift-force-split.md) the [path](../../../continuous-path.md) $t\mapsto g(E(t))$ on $[0,1]$ to a real-valued [path](../../../continuous-path.md) $G$ with $G(0)=0$. Since $g(1)=1$, its endpoint $d=G(1)$ is an integer. On $[0,1)$, $G$ is injective: equality $G(s)=G(t)$ implies $g(E(s))=g(E(t))$, then $E(s)=E(t)$ by injectivity, and hence $s=t$ in this half-open [interval](../../../interval-mathematics.md). A continuous injective [real-valued function](../../../real-valued-function.md) on an [interval](../../../interval-mathematics.md) is strictly monotone.

If $G$ is increasing, $d>0$. It cannot be at least $2$, because the [intermediate value theorem](../../../intermediate-value-theorem.md) would produce $t\in(0,1)$ with $G(t)=1$, giving $g(E(t))=g(1)$ while $E(t)\neq1$. Thus $d=1$. If $G$ is decreasing, the same reasoning gives $d=-1$. Now define

$$
\boxed{K(E(t),s)=\exp\big(2\pi i((1-s)G(t)+sdt)\big).}
$$

At $t=0$ and $t=1$ this has the same value $1$ for every $s$, since $d$ is an integer. Therefore the formula descends continuously from $[0,1]\times[0,1]$ to $S^1\times[0,1]$. At $s=0$ it is $g$; at $s=1$ it is $z\mapsto z^d$. Hence **$g$ is homotopic to the identity or to [complex conjugation](../../../complex-conjugation.md)**, with degree $1$ or $-1$. This is the key property of an [injective self-map of a circle](../../../injective-self-map-of-a-circle.md).

Finally, let $h$ be any continuous injective [circle](../../../circle.md) self-map. Normalize it to $g(z)=\overline{h(1)}h(z)$, which is injective and fixes $1$. If $h$ were not surjective, it would omit some [circle](../../../circle.md) point, so the explicit missing-point construction would make $h$ [null-homotopic](../../../null-homotopic-map.md). Multiplying this [homotopy](../../../homotopy-split.md) by $\overline{h(1)}$ would make $g$ [null-homotopic](../../../null-homotopic-map.md) too. But $g$ is homotopic to the identity or conjugation, neither of which is [null-homotopic](../../../null-homotopic-map.md) by the permitted fact. This contradiction proves **every continuous injective [circle](../../../circle.md) self-map is surjective**. The lifting argument did not assume surjectivity, so the reasoning is not circular.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2010](../../2010-split.md)
3. [Past exam of the topology and groups course of the University of Oxford](../../split.md)
4. [Topology and groups course of the University of Oxford](../../../topology-and-groups-course-of-the-university-of-oxford.md)
5. [Year 3 of the mathematics course of the University of Oxford](../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
