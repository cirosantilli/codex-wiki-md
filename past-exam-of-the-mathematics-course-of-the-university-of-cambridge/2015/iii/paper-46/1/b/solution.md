<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the [shell-restricted scalar propagator](../../../../../../shell-restricted-scalar-propagator.md) be

$$
C_>(x-y)=\int_{\Lambda'<|p|\leq\Lambda}\frac{d^4p}{(2\pi)^4}\frac{e^{ip\cdot(x-y)}}{p^2+m^2}.
$$

Write $\Delta S=S_0[\widehat\phi]+V[\phi,\widehat\phi]$ and average with the normalized Gaussian shell measure. The [cumulant expansion](../../../../../../cumulant-expansion.md) gives

$$
S_{\Lambda'}^{\mathrm{eff}}=S_\Lambda^{\mathrm{eff}}-\log Z_>^0+\langle V\rangle_0-\frac12\left(\langle V^2\rangle_0-\langle V\rangle_0^2\right)+O(g^3).
$$

The subtraction removes [disconnected Feynman diagrams](../../../../../../disconnected-feynman-diagram.md); the logarithm retains [connected Feynman diagrams](../../../../../../connected-feynman-diagram.md) made from shell contractions. This is the [connected shell-contraction expansion](../../../../../../connected-shell-contraction-expansion.md). An external line denotes the background low field, not an additional low-momentum propagator.

<a id="1/b/image-connected-quartic-shell-diagrams-through-second-order-including-vacuum-terms-and-the-two-momentum-support-zeros"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-46-wilsonian-diagrams.png)

**[Figure 1](#1/b/image-connected-quartic-shell-diagrams-through-second-order-including-vacuum-terms-and-the-two-momentum-support-zeros). Connected quartic shell diagrams through second order, including vacuum terms and the two momentum-support zeros**.

At order $g$, panel A is the existing four-field [interaction vertex](../../../../../../interaction-vertex.md). The new shell contractions are B, a [tadpole diagram](../../../../../../tadpole-diagram.md) contributing a two-field vertex, and C, a [Vacuum Feynman diagram](../../../../../../vacuum-feynman-diagram.md) contributing a constant. The Gaussian [functional determinant](../../../../../../functional-determinant.md) in panel L is another field-independent term, of order $g^0$; the original quadratic [kinetic term](../../../../../../kinetic-term.md) and mass term are retained as well.

For completeness, all two-vertex topologies from [Wick contractions](../../../../../../wick-contraction.md) at order $g^2$ are shown. Let $r$ be the number of shell lines joining the vertices and $t_1,t_2$ their numbers of self-contractions. The external-field counts are

$$
e_i=4-r-2t_i,\qquad r\geq1,\qquad t_i\geq0,\qquad e_i\geq0.
$$

Interchanging the two vertices identifies the same topology. Enumerating these conditions gives exactly the following eight possibilities:

- D: $(r,t_1,t_2)=(1,0,0)$, with $(e_1,e_2)=(3,3)$; a six-field vertex kernel.
- E: $(1,0,1)$, with $(3,1)$; a formal four-field kernel, which vanishes for the sharp shell split.
- F: $(1,1,1)$, with $(1,1)$; a formal two-field kernel, which also vanishes for the sharp shell split.
- G: $(2,0,0)$, with $(2,2)$; a four-field vertex kernel.
- H: $(2,0,1)$, with $(2,0)$; a two-field vertex kernel, containing a [tadpole diagram](../../../../../../tadpole-diagram.md).
- I: $(2,1,1)$, with $(0,0)$; a connected [Vacuum Feynman diagram](../../../../../../vacuum-feynman-diagram.md).
- J: $(3,0,0)$, with $(1,1)$; the two-field [sunset diagram](../../../../../../sunset-diagram.md) kernel.
- K: $(4,0,0)$, with $(0,0)$; a connected [Vacuum Feynman diagram](../../../../../../vacuum-feynman-diagram.md) with four joining lines.

The support qualification is important. In E or F, a vertex with one external low field and one bridge also has a tadpole whose two momenta cancel. Conservation forces the bridge momentum to equal that single low momentum, outside the shell. Equivalently, convolution by $C_>$ annihilates $\phi$. This is [momentum-support exclusion for Wilsonian bridge diagrams](../../../../../../momentum-support-exclusion-for-wilsonian-bridge-diagrams.md). D is different: its bridge carries the sum of three low momenta, which can lie in the shell. Its kernel is proportional to $\phi^3(x)C_>(x-y)\phi^3(y)$ and need not vanish. Thus [one-particle-reducible Feynman diagrams](../../../../../../one-particle-reducible-feynman-diagram.md) must not be excluded merely because the object being computed is an effective action.

These kernels need not be local before a [derivative expansion](../../../../../../derivative-expansion.md). Their momentum dependence generates derivative interactions where such an expansion is valid. If all external momenta are sufficiently far below $\Lambda'$, D vanishes too; in particular it does not produce a zero-momentum local $\phi^6$ coupling at order $g^2$. A local six-field term is allowed and is generated at higher orders, for example by a three-vertex shell triangle.

**To all orders, expect every scalar interaction allowed by the original symmetries: arbitrary even powers of the field and their allowed derivative couplings, together with vacuum terms.** The [Z2 symmetry](../../../../../../z2-symmetry.md) $\phi\mapsto-\phi$ excludes odd-field vertices. The original quartic form is therefore not closed under exact Wilsonian integration.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
