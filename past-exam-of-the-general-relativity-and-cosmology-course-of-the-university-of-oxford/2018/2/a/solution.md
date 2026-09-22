<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In coordinates $(ct,r,\phi,z)$ the diagonal [metric tensor](../../../../metric-tensor.md) is $\operatorname{diag}(-1,1,f^2,1)$, and only $g_{\phi\phi}$ depends on position. Substitution into the connection formula gives

$$
\boxed{\Gamma^r{}_{\phi\phi}=-ff',\qquad
\Gamma^\phi{}_{r\phi}=\Gamma^\phi{}_{\phi r}=\frac{f'}f,}
$$

with all other [Christoffel symbols](../../../../christoffel-symbol.md) zero away from singular axes.

Use the explicit [Ricci tensor](../../../../ricci-tensor.md) formula and the [Einstein equation](../../../../einstein-field-equations-split.md) sign printed on the source formula sheet. They give

$$
R_{rr}=\frac{f''}f,\qquad R_{\phi\phi}=ff'',\qquad
\mathcal R=g^{\alpha\beta}R_{\alpha\beta}=2\frac{f''}f.
$$

For example, in $R_{rr}$ the two terms proportional to $(f'/f)^2$ cancel. For $R_{\phi\phi}$ the derivative of $-ff'$ contributes $(f')^2+ff''$, the product terms contribute $-2(f')^2$, and the determinant term contributes $(f')^2$.

**Formula-sheet qualification.** Directly contracting the separately printed [Riemann curvature tensor](../../../../riemann-curvature-tensor-split.md) as instructed on that sheet instead gives $R_{rr}=-f''/f$, the opposite sign. For the concrete example $f(r)=\ell\sin(r/\ell)$, that contraction gives $+1/\ell^2$, whereas the explicit [Ricci tensor](../../../../ricci-tensor.md) formula gives $-1/\ell^2$. The two source formulas cannot both hold with the stated contraction. The calculation here uses the explicit [Ricci tensor](../../../../ricci-tensor.md) formula, whose pairing with the negative [Einstein equation](../../../../einstein-field-equations-split.md) coupling yields the requested [stress-energy tensor](../../../../stress-energy-tensor-split.md).

The desired matter tensor assumes $\Lambda=0$; otherwise the cosmological-constant contribution must also be included. With that assumption,

$$
T_{\alpha\beta}=-\frac{c^4}{8\pi G}
\left(R_{\alpha\beta}-\frac12g_{\alpha\beta}\mathcal R\right),
$$

and raising both indices gives

$$
\boxed{T^{\alpha\beta}=\frac{c^4}{8\pi G}\frac{f''}f
\operatorname{diag}(-1,0,0,1).}
$$

The static observer measures [energy density](../../../../energy-density.md) $T^{00}=-c^4f''/(8\pi Gf)$ and equal-magnitude negative axial [pressure](../../../../pressure-split.md) when that energy is positive. The axial stress is a tension. Keeping the source's curvature sign and its negative Einstein-equation coupling together is essential to this result.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the general relativity and cosmology course of the University of Oxford](../../../split.md)
5. [General relativity and cosmology course of the University of Oxford](../../../../general-relativity-and-cosmology-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
