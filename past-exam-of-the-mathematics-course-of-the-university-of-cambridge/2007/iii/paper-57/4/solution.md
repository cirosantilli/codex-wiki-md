<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Work in the supplied Planck units and write $t=T+\bar T>0$. The nonzero components of the [Kähler metric](../../../../../kahler-metric.md) and its inverse are

$$
K_{T\bar T}=\frac3{t^2},\qquad K_{C\bar C}=1,\qquad K^{T\bar T}=\frac{t^2}3,\qquad K^{C\bar C}=1.
$$

The [Kähler covariant derivatives of a superpotential](../../../../../kahler-covariant-derivative-of-a-superpotential.md) are

$$
D_TW=-\frac{3W}{t},\qquad D_CW=3C^2+\bar C(C^3+B).
$$

In the [supergravity F-term potential](../../../../../supergravity-f-term-potential.md), $K^{T\bar T}|D_TW|^2=3|W|^2$ cancels its negative universal term. This is the [no-scale supergravity](../../../../../no-scale-supergravity.md) identity. The exact answer is therefore

$$
\boxed{V=\frac{e^{|C|^2}}{t^3}\left|3C^2+\bar C(C^3+B)\right|^2\ge0.}
$$

In particular $C=0$ is a global minimum for every $T$ in the domain, with **zero vacuum energy**.

Use the standard convention for a [supergravity auxiliary field](../../../../../supergravity-auxiliary-field.md), $F^i=-e^{K/2}K^{i\bar j}\overline{D_jW}$. In this convention

$$
F^T=e^{K/2}t\bar W,\qquad F^C=-e^{K/2}\left[3\bar C^2+C(\bar C^3+\bar B)\right].
$$

At the $C=0$ minimum these become

$$
\boxed{F^T=\frac{\bar B}{\sqrt t},\qquad F^C=0.}
$$

Thus [supersymmetry breaking](../../../../../supersymmetry-breaking.md) occurs if $B\ne0$, despite the vanishing vacuum energy. Indeed $K_{T\bar T}|F^T|^2=3|B|^2/t^3$ is precisely canceled by the negative [gravitino](../../../../../gravitino.md) contribution. **For $B=0$ the asserted breaking does not occur:** both [supergravity auxiliary fields](../../../../../supergravity-auxiliary-field.md) vanish at $C=0$, so this vacuum is supersymmetric.

For completeness, the full set of finite zero-energy minima includes additional branches. For $C=re^{i\theta}\ne0$, the condition $D_CW=0$ reduces, after factoring $re^{-i\theta}$, to

$$
r(3+r^2)e^{3i\theta}=-B.
$$

For every $B\ne0$ there is a unique positive solution of $r(3+r^2)=|B|$, since the left side increases strictly from zero to infinity. There are three associated phases,

$$
\boxed{r(3+r^2)=|B|,\qquad \theta=\frac{\arg(-B)+2\pi k}{3},\quad k=0,1,2.}
$$

These also give $V=0$, and on each branch $W=3B/(3+r^2)\ne0$. Consequently $F^C=0$ but $F^T\ne0$, so these are also [supersymmetry breaking](../../../../../supersymmetry-breaking.md) [no-scale vacua with a cubic matter superpotential](../../../../../no-scale-vacuum-with-a-cubic-matter-superpotential.md). A supersymmetric finite vacuum would require $D_TW=0$, hence $W=0$, and then $D_CW=3C^2=0$; this is possible only at $C=0$ with $B=0$.

The [scalar potential](../../../../../scalar-potential.md) is independent of $\operatorname{Im}T$ everywhere. On every zero-energy vacuum branch it is also independent of $\operatorname{Re}T$, so **both real components of $T$ are [flat directions of a scalar potential](../../../../../flat-direction-of-a-scalar-potential.md) at the vacuum**. Away from $D_CW=0$, the real direction is not flat: $\partial_tV=-3V/t$, giving a runaway towards $t\to\infty$ rather than a finite positive-energy stationary point. The zero-energy branches have no continuous [flat direction of a scalar potential](../../../../../flat-direction-of-a-scalar-potential.md) in $C$; their allowed $C$ values are isolated. This is why the vacuum does not select a unique numerical [gravitino](../../../../../gravitino.md) mass: the modulus $t$ is unfixed.

The [gravitino mass from a superpotential](../../../../../gravitino-mass-from-a-superpotential.md) is $m_{3/2}=e^{K/2}|W|$. On the conventional $C=0$ branch,

$$
\boxed{m_{3/2}=\frac{|B|}{(T+\bar T)^{3/2}},\qquad V_{\min}=0.}
$$

On a nonzero-$C$ branch it is instead

$$
\boxed{m_{3/2}=\frac{3|B|e^{r^2/2}}{(3+r^2)t^{3/2}}.}
$$

When $B=0$, the only finite zero-energy matter solution is $C=0$ and $m_{3/2}=0$, with unbroken [supersymmetry](../../../../../supersymmetry-split.md). These results exhibit the distinction between vanishing vacuum energy and vanishing [supersymmetry breaking](../../../../../supersymmetry-breaking.md) [auxiliary fields](../../../../../auxiliary-field.md) in a [no-scale supergravity](../../../../../no-scale-supergravity.md) model.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
