<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $M$ be a [closed manifold](../../../../../closed-manifold.md) of even [dimension](../../../../../dimension-vector-space.md) $n=2m$, with a [Riemannian metric](../../../../../riemannian-metric.md) and a [spin structure](../../../../../spin-structure.md). Let $S=S^+\oplus S^-$ be its [spinor bundle](../../../../../spinor-bundle.md), and let $W$ be a [Hermitian vector bundle](../../../../../hermitian-vector-bundle.md) with a [unitary connection](../../../../../unitary-connection.md) of [vector-bundle curvature](../../../../../curvature-form.md) $F^W=(\nabla^W)^2$. We use [Clifford multiplication](../../../../../clifford-multiplication.md) satisfying $c(v)c(w)+c(w)c(v)=-2\langle v,w\rangle$, so the [Twisted Dirac operator](../../../../../twisted-dirac-operator.md)

$$
D_W=\sum_i c(e^i)\nabla^{S\otimes W}_{e_i}
=\begin{pmatrix}0&D_W^-\\D_W^+&0\end{pmatrix}
$$

is [self-adjoint](../../../../../self-adjoint-operator.md) and $D_W^-=(D_W^+)^*$. Here $(e_i)$ is an oriented local [orthonormal basis](../../../../../orthonormal-basis.md) and $(e^i)$ its dual. The [Atiyah-Singer index theorem](../../../../../atiyah-singer-index-theorem.md) in this setting is

$$
\boxed{\operatorname{ind}D_W^+=\int_M\left[\widehat A(R^{TM})\wedge\operatorname{tr}\exp\!\left(\frac{iF^W}{2\pi}\right)\right]_{2m}.}
$$

The second factor is the [Chern character](../../../../../chern-character.md); the first is the [A-hat form](../../../../../a-hat-form.md)

$$
\widehat A(R)=\det{}^{1/2}\!\left(\frac{R/(4\pi i)}{\sinh(R/(4\pi i))}\right).
$$

The square root has constant term one. All functions of the [vector-bundle curvature](../../../../../curvature-form.md) matrices mean [power series](../../../../../power-series.md) truncated above the [dimension](../../../../../dimension-vector-space.md) of $M$. The brackets select the top-degree [differential form](../../../../../differential-form-split.md). The [Bianchi identity](../../../../../bianchi-identity.md) shows that these forms are closed, and [Chern-Weil connection transgression](../../../../../chern-weil-connection-transgression.md) shows that their [de Rham cohomology](../../../../../de-rham-cohomology.md) classes do not depend on the chosen [connections on a vector bundle](../../../../../connection-vector-bundle.md).

The global step is [supersymmetric quantum mechanics](../../../../../supersymmetric-quantum-mechanics.md). On the [Hilbert space](../../../../../hilbert-space-split.md) $L^2(S\otimes W)$, take the grading operator $\Gamma$, the odd supercharge $D_W$, and the nonnegative Hamiltonian $H=D_W^2$. They obey $\Gamma D_W=-D_W\Gamma$ and $D_W^2=H$. The [principal symbol](../../../../../principal-symbol-of-a-partial-differential-equation.md) of $D_W$ is invertible away from the zero covector, so [elliptic regularity](../../../../../elliptic-regularity.md) and [Rellich-Kondrachov compactness theorem](../../../../../rellich-kondrachov-theorem.md) give a smooth discrete [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md) for $H$, finite-dimensional [eigenspaces](../../../../../eigenspace.md), and a [trace-class operator](../../../../../trace-class-operator.md) $e^{-tH}$ for $t>0$. Define its [supertrace](../../../../../supertrace.md) by $\operatorname{Str}A=\operatorname{Tr}(\Gamma A)$.

For every positive [eigenvalue](../../../../../eigenvalue.md) $\lambda$ of $H$, the map $\lambda^{-1/2}D_W$ is an isomorphism between its positive and negative grading [eigenspaces](../../../../../eigenspace.md), with inverse itself. Their contributions to the [supertrace](../../../../../supertrace.md) cancel. The zero [eigenspaces](../../../../../eigenspace.md) are $\ker D_W^+$ and $\ker D_W^-$. Consequently

$$
\operatorname{Str}e^{-tD_W^2}=\dim\ker D_W^+-\dim\ker D_W^-
=\operatorname{ind}D_W^+\qquad(t>0).
$$

This also proves independence of $t$ without differentiating an unbounded operator inside a [trace](../../../../../matrix-trace.md). If $K_t$ is the [heat kernel](../../../../../heat-kernel.md), the [heat kernel trace formula](../../../../../heat-kernel-trace-formula.md) gives

$$
\operatorname{ind}D_W^+=\int_M\operatorname{str}_{S\otimes W}K_t(x,x)\,d\mathrm{vol}_g(x).
$$

The remaining task is to compute this local integrand as $t\downarrow0$.

Fix $p\in M$, use [geodesic normal coordinates](../../../../../geodesic-normal-coordinates.md) $x$, and trivialize $S\otimes W$ by radial [parallel transport](../../../../../parallel-transport.md). Expanding $D_W^2$ at $p$ gives the [Lichnerowicz formula for a twisted Dirac operator](../../../../../lichnerowicz-formula-for-a-twisted-dirac-operator.md):

$$
D_W^2=\nabla^*\nabla+\frac14\operatorname{Scal}+\sum_{i<j}c(e^i)c(e^j)F^W_{ij}.
$$

Indeed the terms with identical indices give the [rough Laplacian](../../../../../rough-laplacian.md). The other terms are $\sum_{i<j}c(e^i)c(e^j)[\nabla_i,\nabla_j]$. Decompose this [vector-bundle curvature](../../../../../curvature-form.md) into spin curvature and $F^W$; substituting the spin curvature into the [Clifford algebra](../../../../../clifford-algebra.md) relations and the algebraic [Bianchi identity](../../../../../bianchi-identity.md) leaves $\operatorname{Scal}/4$. Thus the calculation retains the curvature of the twisting bundle explicitly.

There is an especially strong cancellation in the spinor [supertrace](../../../../../supertrace.md). With $\Gamma=i^mc(e^1)\cdots c(e^{2m})$, every ordered product of distinct Clifford generators of degree less than $2m$ has zero [supertrace](../../../../../supertrace.md), while

$$
\operatorname{str}_S(c(e^1)\cdots c(e^{2m}))=(-2i)^m.
$$

For an even product of lower degree, conjugate $\Gamma$ times that product by a missing Clifford generator: it changes sign, so its [matrix trace](../../../../../matrix-trace.md) is zero. An odd product exchanges the grading summands and also has zero [supertrace](../../../../../supertrace.md). For the full product, $(c(e^1)\cdots c(e^{2m}))^2=(-1)^m$, and $\dim S=2^m$, giving the displayed constant.

To exploit this, identify the [Clifford algebra](../../../../../clifford-algebra.md) as a filtered [vector space](../../../../../vector-space-split.md) with the [exterior algebra](../../../../../exterior-algebra.md) by sending an ordered Clifford product to the corresponding [wedge product of differential forms](../../../../../wedge-product-of-differential-forms.md). Implement [Getzler rescaling](../../../../../getzler-rescaling.md): put $x=\varepsilon y$, $t=\varepsilon^2s$, multiply the degree-$k$ exterior component of the kernel by $\varepsilon^{-k}$, and multiply the whole kernel by $\varepsilon^{2m}$. A derivative and a Clifford generator have rescaling degree one; a coordinate has degree minus one. Clifford contractions lower the degree by two relative to the [wedge product of differential forms](../../../../../wedge-product-of-differential-forms.md), so the leading product becomes [exterior multiplication](../../../../../exterior-multiplication.md).

In the radially parallel frame, the linear Taylor term of the connection is determined by its [vector-bundle curvature](../../../../../curvature-form.md): if $A_i$ is its matrix, then $A_i(x)=\frac12x^jF_{ji}(p)+O(|x|^2)$. To check the coefficient, radial gauge means $x^iA_i=0$, and integration of $x^jF_{ji}$ along the radial segment gives $A_i(x)=\int_0^1s x^jF_{ji}(sx)\,ds$. Combining this formula with the spin representation, the symmetries of [Riemann curvature tensor](../../../../../riemann-curvature-tensor.md), and the [Lichnerowicz formula for a twisted Dirac operator](../../../../../lichnerowicz-formula-for-a-twisted-dirac-operator.md), the rescaled square has leading model

$$
\mathcal H_p=-\sum_i\left(\partial_{y_i}-\frac14\sum_j\mathcal R_{ij}y_j\right)^2+F^W_p.
$$

Here $\mathcal R$ is the skew matrix of tangent-bundle curvature two-forms at $p$; changing the curvature-matrix sign convention changes the sign inside the covariant derivatives but not the determinant below. The coefficients act in $\Lambda T_p^*M\otimes\operatorname{End}(W_p)$. The scalar-curvature term has degree zero and disappears after multiplication by $\varepsilon^2$; the linear spin-connection term and the Clifford action of $F^W$ have degree two and survive. Higher Taylor terms have smaller degree and disappear.

For clarity, the analytic meaning of this limiting calculation is the following. Construct the local [heat kernel expansion](../../../../../heat-kernel-expansion.md) to any fixed order and insert the Taylor expansion of the rescaled coefficients into its transport equations. At each exterior degree, the leading equation is the heat equation of $\mathcal H_p$; the remaining terms acquire positive powers of $\varepsilon$. Equivalently, successive substitutions in

$$
e^{-sP_\varepsilon}-e^{-s\mathcal H_p}
=-\int_0^s e^{-(s-u)P_\varepsilon}(P_\varepsilon-\mathcal H_p)e^{-u\mathcal H_p}\,du
$$

give the same expansion. Polynomial spatial factors are integrable against the local Gaussian kernels, and only finitely many exterior degrees exist. A cutoff outside a fixed normal neighbourhood contributes $O(e^{-c/t})$. Choosing the initial expansion order arbitrarily large bounds its differentiated remainder to any required order. This proves convergence of the rescaled diagonal kernel to the model diagonal kernel, uniformly in $p$ on the [compact manifold](../../../../../compact-manifold.md). Its degree-$2m$ component has no net power of $\varepsilon$, precisely the component detected by the spinor [supertrace](../../../../../supertrace.md).

We can compute the model kernel rather than invoke a local index formula. Set $F=F^W_p$ and seek its kernel from the origin in the form

$$
k_s(y,0)=a(s)\exp\!\left(-\tfrac14 y^TQ(s)y\right)e^{-sF}.
$$

The scalar even exterior coefficients of $\mathcal R$ commute. On this ansatz the rotational first-order term vanishes because $Q$ is a function of $\mathcal R^2$. Expanding the model operator gives $-\sum\partial_i^2+\frac12(\mathcal R y)\cdot\nabla+\frac1{16}y^T\mathcal R^2y+F$, so substitution into the [heat equation](../../../../../heat-equation.md) gives

$$
Q'=\tfrac14\mathcal R^2-Q^2,\qquad\frac{a'}a=-\tfrac12\operatorname{tr}Q.
$$

The Euclidean initial condition $Q(s)\sim s^{-1}I$, $a(s)\sim(4\pi s)^{-m}$ selects

$$
Q(s)=\frac{\mathcal R}{2}\coth\!\left(\frac{s\mathcal R}{2}\right),\qquad
a(s)=(4\pi s)^{-m}\det{}^{1/2}\!\left(\frac{s\mathcal R/2}{\sinh(s\mathcal R/2)}\right).
$$

These expressions have well-defined [power series](../../../../../power-series.md) at $\mathcal R=0$. This is the curvature version of the Gaussian calculation underlying the [Mehler formula for Hermite functions](../../../../../mehler-formula-for-hermite-functions.md).

At $s=1$, $y=0$, multiply the top exterior coefficient by the spinor [supertrace](../../../../../supertrace.md) constant. Since $(4\pi)^{-m}(-2i)^m=(2\pi i)^{-m}$, and every curvature factor is a two-form, the result is

$$
\lim_{t\downarrow0}\operatorname{str}K_t(p,p)\,d\mathrm{vol}_g(p)
=\left[\det{}^{1/2}\!\left(\frac{R^{TM}/(4\pi i)}{\sinh(R^{TM}/(4\pi i))}\right)
\operatorname{tr}\exp\!\left(-\frac{F^W}{2\pi i}\right)\right]_{2m}(p).
$$

Integration and the constant [supertrace](../../../../../supertrace.md) established above prove the boxed [Atiyah-Singer index theorem](../../../../../atiyah-singer-index-theorem.md). The mechanism is that odd symmetry pairs the nonzero spectrum globally, while the Clifford filtration makes the surviving local contribution an explicitly solvable curvature oscillator. Odd-dimensional spin [Dirac operators](../../../../../dirac-operator.md) have no canonical chiral index of this type; their self-adjoint [Fredholm index](../../../../../fredholm-index.md) is zero. For comparison of normalization conventions, [Raphaël Ponge's local index calculation](https://arxiv.org/pdf/math/0211333) writes the same unnormalized curvature model and spinor supertrace constant.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
