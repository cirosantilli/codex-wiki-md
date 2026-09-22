<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use Cartesian coordinates $x^a=(t,x,y,z)$ with $c=1$ and $\eta_{ab}=\operatorname{diag}(1,-1,-1,-1)$. Spatial dot and [cross products](../../../../cross-product.md) below use the Euclidean three-metric. The alternating [tensor](../../../../tensor.md) is given the orientation $\epsilon^{0123}=+1$.

**[Vector](../../../../vector.md) and [covector](../../../../covector.md) transformation.** The [vector](../../../../vector.md) $A=A^b\partial_b$ is independent of coordinates, and the [chain rule](../../../../chain-rule.md) gives $\partial_b=(\partial x'^a/\partial x^b)\partial'_a$. Likewise the [one-form](../../../../one-form.md) $A_bdx^b$ is independent of coordinates. Comparing coefficients proves

$$
\boxed{A'^a=\frac{\partial x'^a}{\partial x^b}A^b,
\qquad A'_a=\frac{\partial x^b}{\partial x'^a}A_b.}
$$

Their contraction $A_a B^a$ is unchanged because the forward and inverse Jacobians cancel. Here lowering an index uses the metric, not an identification of the numerical upper and lower components.

**Why antisymmetrization matters.** Write $J^c{}_a=\partial x^c/\partial x'^a$. Differentiating the [covector](../../../../covector.md) law gives

$$
\partial'_a A'_b
=J^c{}_aJ^d{}_b\,\partial_c A_d
+\frac{\partial^2x^d}{\partial x'^a\partial x'^b}A_d.
$$

The last term obstructs the general [tensor](../../../../tensor.md) transformation law. It is symmetric in $a,b$, so it cancels from $\partial'_aA'_b-\partial'_bA'_a$. Therefore

$$
\boxed{F'_{ab}=J^c{}_aJ^d{}_bF_{cd}.}
$$

Equivalently $F=dA$ is the [exterior derivative](../../../../exterior-derivative.md) of the [electromagnetic four-potential](../../../../electromagnetic-four-potential.md) [one-form](../../../../one-form.md). The statement that $\partial_aA_b$ is not a [tensor](../../../../tensor.md) needs a qualification: **under affine Cartesian [Lorentz transformations](../../../../lorentz-transformation.md) it does transform tensorially**, because the second derivatives vanish. The failure concerns arbitrary nonlinear coordinate changes, including curvilinear coordinates in flat spacetime. This distinction is precisely the difference between general covariance and covariance under the restricted inertial-frame transformations.[Section 2, Manifolds, equations 2.26–2.27: the extra second-derivative term and its cancellation under antisymmetrization](../../../../lecture-notes-on-general-relativity-by-sean-m-carroll.md)

**Electric and magnetic components.** Choose $A^a=(\Phi,\mathbf A)$, so $A_a=(\Phi,-\mathbf A)$, $\mathbf E=-\boldsymbol\nabla\Phi-\partial_t\mathbf A$ and $\mathbf B=\boldsymbol\nabla\times\mathbf A$. Then

$$
F_{0i}=\partial_t(-A_i^{\rm spatial})-\partial_i\Phi=E_i,
\qquad F_{ij}=-\epsilon_{ijk}B_k.
$$

Thus the lower-index field [tensor](../../../../tensor.md) is

$$
F_{ab}=\begin{pmatrix}
0&E_x&E_y&E_z\\
-E_x&0&-B_z&B_y\\
-E_y&B_z&0&-B_x\\
-E_z&-B_y&B_x&0
\end{pmatrix}.
$$

This is a derived component representation of the field, with the source's sign convention.

**Raised indices and the first invariant.** Raising both indices changes the time-space signs and leaves the spatial block unchanged:

$$
\boxed{F^{ab}=\begin{pmatrix}
0&-E_x&-E_y&-E_z\\
E_x&0&-B_z&B_y\\
E_y&B_z&0&-B_x\\
E_z&-B_y&B_x&0
\end{pmatrix}.}
$$

In the [scalar](../../../../scalar.md) contraction, each independent antisymmetric pair is counted twice, giving

$$
\boxed{F_{ab}F^{ab}=2(B^2-E^2).}
$$

Under a [Lorentz transformation](../../../../lorentz-transformation.md) each inverse transformation from a lower index cancels its matching transformation from an upper index, leaving the same [scalar](../../../../scalar.md). In particular a [plane electromagnetic wave](../../../../plane-electromagnetic-wave.md) has $E=B$ in these units and makes this invariant vanish, while a pure [electric field](../../../../electric-field-split.md) makes it negative.

**The printed dual convention.** The PDF explicitly defines ${}^*F^{ab}=\epsilon^{abcd}F_{cd}$, with no $1/2$. Each independent pair therefore contributes twice: for example ${}^*F^{01}=F_{23}-F_{32}=-2B_x$. The complete result is

$$
\boxed{{}^*F^{ab}=2\begin{pmatrix}
0&-B_x&-B_y&-B_z\\
B_x&0&E_z&-E_y\\
B_y&-E_z&0&E_x\\
B_z&E_y&-E_x&0
\end{pmatrix},\qquad {}^*F^{ab}F_{ab}=-8\mathbf E\cdot\mathbf B.}
$$

The time-space pairs contribute $-4\mathbf E\cdot\mathbf B$ and the spatial pairs contribute another $-4\mathbf E\cdot\mathbf B$. The conventional Hodge dual includes $1/2$ and would instead give the contraction $-4\mathbf E\cdot\mathbf B$; it must not silently replace this paper's definition. With fixed orientation the latter contraction is a [pseudoscalar](../../../../pseudoscalar.md): invariant under proper [Lorentz transformations](../../../../lorentz-transformation.md) but odd under orientation reversal if compared using a fixed alternating symbol.

**[Energy density](../../../../energy-density.md) and flux.** Substitution into the given mixed stress-energy [tensor](../../../../tensor.md) yields

$$
\boxed{T^0{}_0=\frac{E^2+B^2}{2\mu_0},\qquad
T^0{}_i=-\frac{(\mathbf E\times\mathbf B)_i}{\mu_0}.}
$$

For the first formula, $F^{0c}F_{0c}=-E^2$ and $F_{cd}F^{cd}/4=(B^2-E^2)/2$. For the second, $F^{0j}F_{ij}=(\mathbf E\times\mathbf B)_i$. The minus sign on $T^0{}_i$ arises from its lowered spatial index; it does not reverse the physical [energy](../../../../energy-split.md) flow. Raising that index gives $T^{0i}=S_i$, and symmetry gives $T^{i0}=S_i$, with $\mathbf S=\mathbf E\times\mathbf B/\mu_0$ the [Poynting vector](../../../../poynting-vector.md) in $c=1$ units. Thus $T^{00}$ is [energy density](../../../../energy-density.md) and $T^{i0}$ represents [energy](../../../../energy-split.md) flux. In SI coordinates $x^0=ct$, restore $T^{0i}=S_i/c$ and $T^{00}=(\epsilon_0 E_{\rm SI}^2+B^2/\mu_0)/2$, with $\epsilon_0\mu_0c^2=1$. This keeps the mixed-index signs and the units distinct.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
4. [Past exam of the relativity course of the University of Cambridge](../../../split.md)
5. [Relativity course of the University of Cambridge](../../../../relativity-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
