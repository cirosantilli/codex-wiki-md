<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let the flow direction be $x$, the gradient direction $y$, and the vorticity direction $z$, with [simple shear flow](../../../../../../simple-shear-flow.md) $u=(s y,0,0)$ and signed [shear rate](../../../../../../shear-rate.md) $s=\dot\gamma$. Use the gradient convention established in part (a):

$$
\omega=\begin{pmatrix}0&-s&0\\s&0&0\\0&0&0\end{pmatrix},\qquad
\dot\gamma=\begin{pmatrix}0&s&0\\s&0&0\\0&0&0\end{pmatrix}.
$$

At steady homogeneous shear the ordinary time derivative and advection vanish. Put $X=\sigma_{xx}$, $Y=\sigma_{yy}$ and $S=\sigma_{xy}$. The [corotational Maxwell fluid](../../../../../../corotational-maxwell-fluid.md) law then gives

$$
X-\lambda s S=0,\qquad Y+\lambda s S=0,\qquad
S+\frac{\lambda s}{2}(X-Y)=\mu s.
$$

The $zz$ equation gives $\sigma_{zz}=0$, and the unforced $xz,yz$ equations force those components to zero. Solving the three displayed equations gives the [steady shear of a corotational Maxwell fluid](../../../../../../steady-shear-of-a-corotational-maxwell-fluid.md):

$$
S=\frac{\mu s}{1+\lambda^2s^2},\qquad
X=\frac{\mu\lambda s^2}{1+\lambda^2s^2},\qquad Y=-X.
$$

The [deviatoric stress](../../../../../../deviatoric-stress.md) is indeed traceless. Its isotropic pressure contribution is irrelevant to either shear viscosity or a [normal-stress difference](../../../../../../normal-stress-difference.md).

Consequently the steady [shear viscosity](../../../../../../dynamic-viscosity.md) is

$$
\boxed{\eta_{\rm sh}(s)=\frac{S}{s}=\frac{\mu}{1+\lambda^2s^2},\qquad \eta_{\rm sh}(0)=\mu.}
$$

For $s>0$, $d\eta_{\rm sh}/ds=-2\mu\lambda^2s/(1+\lambda^2s^2)^2<0$ when $\mu,\lambda>0$; it decreases with $|s|$ and tends to zero at large rate. This proves [shear thinning](../../../../../../shear-thinning.md) directly, without confusing a decreasing viscosity with a necessarily decreasing shear stress.

With the standard definitions $N_1=\sigma_{xx}-\sigma_{yy}$ and $N_2=\sigma_{yy}-\sigma_{zz}$,

$$
\boxed{N_1=\frac{2\mu\lambda s^2}{1+\lambda^2s^2}>0,\qquad
N_2=-\frac{\mu\lambda s^2}{1+\lambda^2s^2}=-\frac12N_1<0.}
$$

At zero shear both vanish; at small shear they are quadratic, consistently with part (b). The signs and the fact $|N_2|<N_1$ agree qualitatively with many polymeric-fluid experiments. However the fixed ratio $|N_2|/N_1=1/2$ often overestimates the measured second difference and cannot capture variation of that ratio with material and shear rate. For example, [measurements on polyethylene](https://onlinelibrary.wiley.com/doi/full/10.1002/app.52094) show a smaller, rate-dependent relative second normal-stress difference. Thus **the qualitative normal-stress signs are reasonable, but the predicted relative magnitude is not generally quantitatively satisfactory**; these signs are not a universal statement about every non-Newtonian fluid.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
