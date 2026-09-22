<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [superficial degree of divergence](../../../../../superficial-degree-of-divergence.md) is the power of a common large-momentum scale obtained by scaling all independent internal momenta together, before cancellations or subtraction of divergent subdiagrams. In a [scalar field theory](../../../../../scalar-field-theory-split.md) with a standard quadratic kinetic term and non-derivative interactions, each [loop momentum](../../../../../loop-momentum.md) integral supplies $d$ powers of momentum and each internal [propagator](../../../../../propagator.md) supplies minus two. Thus

$$
D=dL-2I.
$$

For a connected [Feynman diagram](../../../../../feynman-diagram.md), counting vertex half-edges and applying the stated identity for the [loop order](../../../../../loop-order.md) gives

$$
2I+E=\sum_n nV_n,\qquad I=L+V-1,\qquad V=\sum_n V_n.
$$

It follows that $D=(d-2)L-2V+2$. Meanwhile, $\sum_n(n-4)V_n=2I+E-4V=2L-2V+E-2$. Substitution proves

$$
\boxed{D=(d-4)L+\sum_n(n-4)V_n-E+4.}
$$

This [power counting in quantum field theory](../../../../../power-counting-in-quantum-field-theory.md) concerns the overall scaling: even a [Feynman diagram](../../../../../feynman-diagram.md) with $D<0$ can contain divergent subdiagrams, and cancellations may improve convergence when $D\geq0$.

The canonical [mass dimensions](../../../../../mass-dimension.md) are $[\phi]=(d-2)/2$ and $[g_n]=d-n(d-2)/2$. A finite polynomial [scalar field theory](../../../../../scalar-field-theory-split.md) has power-counting [renormalizability](../../../../../renormalizable-quantum-field-theory.md) when its interactions have nonnegative [mass dimensions](../../../../../mass-dimension.md) and the allowed local [counterterms](../../../../../counterterm.md) form a finite set closed under subtraction of divergent subdiagrams. For $d>2$, non-derivative interactions therefore satisfy $n\leq2d/(d-2)$. Equivalently,

$$
D=d-\frac{d-2}{2}E-\sum_n[g_n]V_n,
$$

so adding vertices of such interactions cannot force an indefinitely increasing number of external legs or derivatives in divergent [counterterms](../../../../../counterterm.md). In dimensions $d\leq2$ a fixed finite polynomial still has this favorable [power counting in quantum field theory](../../../../../power-counting-in-quantum-field-theory.md); the displayed upper bound on $n$ is intended only for $d>2$.

For [six-dimensional cubic scalar field theory](../../../../../six-dimensional-cubic-scalar-field-theory.md), $3V=2I+E$ and $L=I-V+1$ yield

$$
\boxed{D=6-2E.}
$$

The coupling $g$ has zero [mass dimension](../../../../../mass-dimension.md). The possible overall divergences have $E\leq3$: vacuum energy, a linear [tadpole diagram](../../../../../tadpole-diagram.md) term, a mass term, a kinetic term, and a cubic interaction. These are finitely many local [counterterms](../../../../../counterterm.md). Divergent subdiagrams of higher-point [Feynman diagrams](../../../../../feynman-diagram.md) are removed by the same [counterterms](../../../../../counterterm.md), establishing [perturbative renormalizability of cubic scalar theory in six dimensions](../../../../../perturbative-renormalizability-of-cubic-scalar-theory-in-six-dimensions.md). A real cubic potential is unbounded below, so this claim is one of [perturbative quantum field theory](../../../../../perturbative-quantum-field-theory-split.md), not a claim that the polynomial defines a stable nonperturbative vacuum.

After [Wick rotation](../../../../../wick-rotation.md), use the [Euclidean action](../../../../../euclidean-action.md) with positive kinetic and mass terms and interaction $g\phi^3/3!$. The Euclidean momentum-space [Feynman rules](../../../../../feynman-rule.md) are: an internal [scalar propagator](../../../../../scalar-propagator.md) $1/(k^2+m^2)$, a vertex $-g$, momentum conservation at each vertex, integration $d^6k/(2\pi)^6$ for each independent loop, and division by the [Feynman-diagram symmetry factor](../../../../../feynman-diagram-symmetry-factor.md). Strip the overall momentum-conserving delta function and external [propagators](../../../../../propagator.md) when computing an [amputated Green's function](../../../../../amputated-connected-correlation-function.md).

The [one-particle-irreducible two-point vertex](../../../../../one-particle-irreducible-two-point-vertex.md) at one loop is the bubble:

<a id="2/image-one-loop-cubic-scalar-two-point-bubble-with-symmetry-factor-two"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-48-self-energy.png)

**[Figure 2](#2/image-one-loop-cubic-scalar-two-point-bubble-with-symmetry-factor-two). One-loop cubic scalar two-point bubble with symmetry factor two**.

Interchanging its two internal lines is an automorphism, giving [Feynman-diagram symmetry factor](../../../../../feynman-diagram-symmetry-factor.md) two. In the normalization of the printed Minkowski [amputated Green's function](../../../../../amputated-connected-correlation-function.md), the two vertices contribute $(-ig)^2$, the two internal [propagators](../../../../../propagator.md) contribute $(-i)^2$, and [Wick rotation](../../../../../wick-rotation.md) supplies the overall $i$ already factored out there. Thus the Euclidean bubble contribution is

$$
\boxed{\widehat F_2^{(1)}(p)=\frac{g^2}{2}\int\frac{d^6k}{(2\pi)^6}\frac1{(k^2+m^2)((k+p)^2+m^2)}.}
$$

For this [self-energy](../../../../../self-energy.md) calculation we impose a vanishing [one-point function](../../../../../one-point-correlation-function.md), so [tadpole diagram](../../../../../tadpole-diagram.md) insertions are canceled by the linear [counterterm](../../../../../counterterm.md). Without that convention a connected but [one-particle-reducible Feynman diagram](../../../../../one-particle-reducible-feynman-diagram.md) with a tadpole insertion is also possible: both external legs attach to one vertex, a zero-momentum line joins it to a second vertex, and that second vertex has a self-loop. Its amputated contribution is $g^2/(2m^2)\int d^6k/[(2\pi)^6(k^2+m^2)]$, independent of $p$. It is not the bubble drawn above; keeping it without a tadpole subtraction would add this constant to the full amputated answer.

To find the bubble's local divergence, put $K=k^2+m^2$ and expand at large $|k|$:

$$
\frac1{K(K+2k\cdot p+p^2)}=\frac1{K^2}-\frac{2k\cdot p+p^2}{K^3}+\frac{(2k\cdot p+p^2)^2}{K^4}+\cdots.
$$

Odd terms vanish under the angular integral. Rotational symmetry gives $\langle(k\cdot p)^2\rangle=k^2p^2/6$. The terms through order $p^2$ are therefore

$$
\frac1{K^2}+p^2\left(-\frac1{K^3}+\frac{2k^2}{3K^4}\right),
$$

and the $p^2$ coefficient approaches $-1/(3k^6)$. Terms of order $p^4$ and higher are integrable at infinity in six dimensions; subtracting the two displayed terms leaves an ultraviolet-convergent integral. Hence the divergent part is **a local polynomial $A p^2+B$**, with momentum-independent coefficients. For example, when $m^2>0$ its logarithmically divergent coefficient is

$$
A_{\rm div}=-\frac{g^2}{768\pi^3}\log\frac{\Lambda^2}{m^2}.
$$

Changing the reference scale in this logarithm only changes a finite local term.

At zero external momentum the spherical [ultraviolet cutoff](../../../../../ultraviolet-cutoff.md) and $\operatorname{Vol}(S^5)=\pi^3$ give

$$
B_\Lambda=\widehat F_2^{(1)}(0)=\frac{g^2}{128\pi^3}\int_0^\Lambda\frac{k^5\,dk}{(k^2+m^2)^2}.
$$

With $u=k^2$, integrate $u^2/(u+m^2)^2=1-2m^2/(u+m^2)+m^4/(u+m^2)^2$. This gives the [momentum-cutoff two-point function in six-dimensional cubic scalar theory](../../../../../momentum-cutoff-two-point-function-in-six-dimensional-cubic-scalar-theory.md)

$$
\boxed{B_\Lambda=\frac{g^2}{256\pi^3}\left[\Lambda^2-2m^2\log\left(1+\frac{\Lambda^2}{m^2}\right)+\frac{m^2\Lambda^2}{\Lambda^2+m^2}\right].}
$$

In particular, the divergent part of this constant is

$$
\boxed{B_{\rm div}=\frac{g^2}{256\pi^3}\left[\Lambda^2-2m^2\log\frac{\Lambda^2}{m^2}\right],}
$$

while the last term in $B_\Lambda$ tends to a finite constant. For $m=0$ the zero-momentum integral gives $B_\Lambda=g^2\Lambda^2/(256\pi^3)$ directly. The finite parts of a local subtraction can depend on the [regularization](../../../../../regularization.md) prescription; the conclusion about mass and kinetic [counterterms](../../../../../counterterm.md) does not.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
