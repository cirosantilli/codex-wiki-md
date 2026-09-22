<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

An [asymptotically flat spacetime](../../../../../asymptotically-flat-spacetime.md) at [future null infinity](../../../../../future-null-infinity.md) admits a smooth [conformal completion](../../../../../conformal-completion.md) $(\overline{\mathcal M},\bar g)$ with the following properties. The physical spacetime $\mathcal M$ is the interior of $\overline{\mathcal M}$, its metric obeys

$$
\bar g_{ab}=\Omega^2g_{ab},
$$

and the boundary component $\mathcal I^+$ satisfies $\Omega=0$ and $d\Omega\ne0$. Every future-directed outgoing null geodesic has an endpoint there, the generators of $\mathcal I^+$ are complete, and in four spacetime dimensions $\mathcal I^+\simeq\mathbb R\times S^2$. The physical [Einstein field equations](../../../../../einstein-field-equations.md) are vacuum in a neighborhood of this boundary.

Let $n_a=\bar\nabla_a\Omega$. Multiplying the supplied conformal Ricci relation by $\Omega^2$, using $R_{ab}=0$, and taking the limit to $\mathcal I^+$ gives

$$
0=-3\bar g_{ab}n^cn_c,
\qquad
\boxed{n^an_a=0\quad\hbox{on }\mathcal I^+}.
$$

The boundary normal is therefore null. Since a null normal is also tangent to its hypersurface, $n^a$ generates $\mathcal I^+$.

Smoothness makes $s=\Omega^{-1}n^2$ finite at the boundary. Multiplication of the same vacuum equation by $\Omega$ gives there

$$
2\bar\nabla_an_b+\bar g_{ab}(\bar\Box\Omega-3s)=0.
$$

Taking the trace yields $s=\tfrac12\bar\Box\Omega$, and substitution gives

$$
\bar\nabla_an_b=\frac14\bar g_{ab}\bar\Box\Omega.
$$

The remaining freedom $\Omega\mapsto\omega\Omega$ can be used to impose $\bar\Box\Omega=0$ on $\mathcal I^+$. In this conformal gauge, $\bar\nabla_an_b=0$ there, so the generators are affinely parametrized, expansion-free null geodesics of the unphysical metric.

Choose a generator coordinate $u$, the defining function $\Omega$, and angular coordinates $x^A$ whose leading metric $q_{AB}$ is the round metric on the [unit sphere](../../../../../unit-sphere.md). After the conformal and coordinate choices above, the leading unphysical metric is

$$
\bar g=2\,du\,d\Omega+q_{AB}dx^Adx^B+O(\Omega),
$$

with the Minkowski term $-\Omega^2du^2$ entering at the next relevant order. Setting $r=\Omega^{-1}$ recovers the physical asymptotic form

$$
g=-du^2-2\,du\,dr+r^2q_{AB}dx^Adx^B
+\text{terms lower by powers of }r.
$$

The displayed leading metric is [Minkowski spacetime](../../../../../minkowski-spacetime.md) in outgoing null coordinates. Smooth conformal extendibility controls the lower-order corrections, while the vacuum equations constrain them to the radiative Bondi--Sachs expansion. This is the precise sense in which the permitted spacetimes approach Minkowski spacetime near $\mathcal I^+$ while still allowing outgoing gravitational radiation.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 311](../../paper-311-split.md)
3. [Iii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
