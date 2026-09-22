<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For small [displacement](../../../../displacement.md) [gradients](../../../../gradient.md) write $F=I+H$. [Taylor expansion](../../../../taylor-expansion.md) around the stress-free reference state gives

$$
W(I+H)=W(I)+\frac12C_{i\alpha j\beta}H_{i\alpha}H_{j\beta}+o(|H|^2),
\qquad C_{i\alpha j\beta}=D^2W(I)_{i\alpha j\beta}.
$$

The linear term vanishes because $DW(I)=0$. Drop the irrelevant constant and retain the quadratic term:

$$
\boxed{W^{\mathrm{lin}}(H)=\frac12C_{i\alpha j\beta}H_{i\alpha}H_{j\beta}.}
$$

The major symmetry $\boxed{C_{i\alpha j\beta}=C_{j\beta i\alpha}}$ follows from equality of mixed second [derivatives](../../../../derivative.md). For a skew matrix $K$, stress covariance along $e^{tK}$ gives

$$
\widehat T(e^{tK})=e^{tK}\widehat T(I)=0.
$$

Differentiation at zero yields $D\widehat T(I)[K]=C[K]=0$. Thus $C_{i\alpha j\beta}K_{j\beta}=0$ for every skew matrix, which forces the input minor symmetry $C_{i\alpha j\beta}=C_{i\alpha\beta j}$. Combining it with the major symmetry gives the output minor symmetry as well:

$$
\boxed{C_{i\alpha j\beta}=C_{\alpha i j\beta}=C_{i\alpha\beta j}.}
$$

These identify reference and spatial indices at $F=I$. Decompose $H=e+K$ into symmetric and skew parts. Since $C[K]=0$ and the major symmetry also eliminates the other cross term,

$$
\boxed{W^{\mathrm{lin}}(H)=\tfrac12C[e,e],\qquad e=(H+H^T)/2.}
$$

Thus infinitesimal rotations cost no energy in the quadratic approximation.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
