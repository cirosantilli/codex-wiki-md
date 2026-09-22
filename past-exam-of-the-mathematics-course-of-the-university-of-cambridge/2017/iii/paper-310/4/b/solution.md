<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [first Hubble slow-roll parameter](../../../../../../first-hubble-slow-roll-parameter.md) measures the fractional change of $H$ per [number of e-folds](../../../../../../number-of-e-folds.md), and the [second Hubble slow-roll parameter](../../../../../../second-hubble-slow-roll-parameter.md) measures the fractional change of the first parameter. Since $d\log a/dt=H$,

$$
\boxed{\epsilon=-\frac{\dot H}{H^2},\qquad\eta=\frac{\dot\epsilon}{H\epsilon}.}
$$

For a canonical [inflaton](../../../../../../inflaton.md), $\epsilon=\dot\phi^2/(2M_{\rm Pl}^2H^2)\geq0$. Expanding [cosmic inflation](../../../../../../cosmic-inflation-split.md) means $\ddot a>0$, equivalently $\boxed{\epsilon<1}$ because $\ddot a/a=H^2(1-\epsilon)$. Small $\eta$ is not required for accelerated expansion itself, but helps maintain the [slow-roll approximation](../../../../../../slow-roll-approximation.md) over many e-folds. Its logarithmic definition assumes $\epsilon>0$; in exact de Sitter expansion it is undefined unless interpreted as a limit.

For conventional [slow-roll inflation](../../../../../../slow-roll-approximation.md), assume $\dot\phi^2\ll V$, $|\ddot\phi|\ll3H|\dot\phi|$, a smooth positive [scalar potential](../../../../../../scalar-potential.md), and slowly varying small parameters. The [Friedmann equation](../../../../../../friedmann-equations.md) and [inflaton equation of motion](../../../../../../inflaton-equation-of-motion.md) then reduce to

$$
\boxed{H^2\simeq\frac{V}{3M_{\rm Pl}^2},\qquad3H\dot\phi\simeq-V_{,\phi}.}
$$

Substitute these in the exact expression for $\epsilon$:

$$
\epsilon\simeq\frac{V_{,\phi}^2}{18M_{\rm Pl}^2H^4}=\frac{M_{\rm Pl}^2}{2}\left(\frac{V_{,\phi}}V\right)^2\equiv\epsilon_V.
$$

To obtain the [potential and Hubble slow-roll parameter relation](../../../../../../potential-and-hubble-slow-roll-parameter-relation.md), differentiate $\log\epsilon_V$ along the slow-roll trajectory $\dot\phi/H\simeq-M_{\rm Pl}^2V_{,\phi}/V$:

$$
\eta\simeq2\left(\frac{V_{,\phi\phi}}{V_{,\phi}}-\frac{V_{,\phi}}V\right)\frac{\dot\phi}{H}
=4\epsilon_V-2M_{\rm Pl}^2\frac{V_{,\phi\phi}}V.
$$

Hence

$$
\boxed{\epsilon\simeq\epsilon_V,\qquad2\epsilon-\frac\eta2\simeq\eta_V=M_{\rm Pl}^2\frac{V_{,\phi\phi}}V.}
$$

The second quantity on the right is the [second potential slow-roll parameter](../../../../../../second-potential-slow-roll-parameter.md), not the logarithmic Hubble-flow $\eta$ itself. Consistency usually requires $\epsilon_V\ll1$ and $|\eta_V|\ll1$; identities involving division by $V_{,\phi}$ are used on rolling intervals and interpreted by limiting values at stationary points.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
