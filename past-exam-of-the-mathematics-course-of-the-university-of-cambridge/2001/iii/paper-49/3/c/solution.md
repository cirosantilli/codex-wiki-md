<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For [uniaxial extensional flow](../../../../../../uniaxial-extensional-flow.md) use $\mathbf v=\dot\gamma(x,-y/2,-z/2)$, so $L=E=\dot\gamma\operatorname{diag}(1,-1/2,-1/2)$. Again put $q=\dot\gamma\tau$ and $f=1+\alpha\operatorname{tr}A$. A steady diagonal tensor has

$$
(f-2q)a_{11}=2q,\qquad(f+q)a_{22}=(f+q)a_{33}=-q.
$$

Set $T=f-2q$. Then

$$
a_{11}=\frac{2q}{T},\qquad a_{22}=a_{33}=-\frac{q}{T+3q},\qquad
\operatorname{tr}A=\frac{6q^2}{T(T+3q)}.
$$

Since $f-1=\alpha\operatorname{tr}A$ and $f=T+2q$, multiplication gives

$$
\boxed{T(T+2q-1)(T+3q)=6\alpha q^2.}
$$

This is the cubic for [uniaxial extension of an affine linear PTT fluid](../../../../../../uniaxial-extension-of-an-affine-linear-ptt-fluid.md). For $\alpha>0$, choose its physical root $T>\max(0,1-2q)$, continuous from $T=1$ at rest. The product on the left grows strictly from zero to infinity in that interval, so this root is unique. The other algebraic roots need not describe an admissible steady material state.

The [extensional viscosity](../../../../../../extensional-viscosity.md) is the axial-minus-transverse normal stress divided by the principal extension rate. Isotropic pressure cancels, leaving

$$
\eta_E=\frac{G_0(a_{11}-a_{22})}{\dot\gamma}
=G_0\tau\left(\frac2T+\frac1{T+3q}\right).
$$

At small $q$, $f=1+6\alpha q^2+O(q^3)$ and $T=1-2q+O(q^2)$. Thus

$$
\boxed{\eta_E\longrightarrow3G_0\tau\qquad(q\to0),}
$$

the [Trouton ratio](../../../../../../trouton-ratio.md) of three relative to the [zero-shear viscosity](../../../../../../zero-shear-viscosity.md). At large $q$ with fixed $\alpha>0$, the positive cubic root remains bounded and tends to $\alpha$: dividing the cubic by $6q^2$ gives $T[1+O(q^{-1})]=\alpha$. Therefore

$$
\boxed{\eta_E\longrightarrow\frac{2G_0\tau}{\alpha}\qquad(q\to\infty,\ \alpha>0).}
$$

The nonlinear relaxation prevents the divergent high-rate response of the affine Maxwell model. If $\alpha=0$, the physically stable steady branch instead has $f=1$ and ends at $q=1/2$; no finite positive high-rate limit follows. The finite plateau consequently presumes the usual positive PTT relaxation parameter, as well as $G_0,\tau>0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
