<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [inextensible fibre constraint](../../../../../inextensible-fibre-constraint.md) gives $|\mathbf x_{,1}|=1$. Write the fibre direction and its transverse unit direction as

$$
e=(\cos\theta,\sin\theta),\qquad n=(-\sin\theta,\cos\theta).
$$

Then $x_{1,1}=\cos\theta$ and $x_{2,1}=\sin\theta$. In [plane strain](../../../../../plane-strain.md), [incompressibility](../../../../../incompressible-flow.md) gives $\det F=1$. Decomposing the second column of the [deformation gradient](../../../../../deformation-gradient.md) along $e,n$ therefore gives $\mathbf x_{,2}=\gamma e+n$, where $\gamma=\mathbf x_{,2}\cdot e$. Hence

$$
\boxed{F=R(\theta)\begin{pmatrix}1&\gamma\\0&1\end{pmatrix}.}
$$

This is a local rotation followed by [simple shear](../../../../../simple-shear.md).

The compatibility of the [deformation map](../../../../../deformation-map.md) requires $\mathbf x_{,12}=\mathbf x_{,21}$. Since $e_{,j}=\theta_{,j}n$ and $n_{,j}=-\theta_{,j}e$, this is

$$
\theta_{,2}n=(\gamma_{,1}-\theta_{,1})e+\gamma\theta_{,1}n.
$$

Taking components gives the compatibility relations for [incompressible inextensible-fibre plane strain](../../../../../incompressible-inextensible-fibre-plane-strain.md):

$$
\boxed{\gamma_{,1}=\theta_{,1},\qquad\theta_{,2}=\gamma\theta_{,1},\qquad\gamma=\theta+f(X_2).}
$$

Along a reference curve,

$$
\frac{d\theta}{ds}=\theta_{,1}\left(\frac{dX_1}{ds}+\gamma\frac{dX_2}{ds}\right).
$$

Thus $\theta$ is constant when $dX_2/dX_1=-1/\gamma$. The equivalent condition $dX_1+\gamma\,dX_2=0$ also covers $\gamma=0$. Its current tangent is proportional to $F(-\gamma,1)^T=n$, so these transverse curves are straight wherever the deformation is regular.

To construct the stress with zero [body force](../../../../../body-force.md), specify the local [shear stress](../../../../../shear-stress.md) $h$ as the material's function or functional of $\gamma$ under [simple shear](../../../../../simple-shear.md). The normal stresses are constraint reactions: [incompressibility](../../../../../incompressible-flow.md) supplies pressure, and the [inextensible fibre constraint](../../../../../inextensible-fibre-constraint.md) supplies fibre tension. Write

$$
\sigma=s\,e\otimes e+h(e\otimes n+n\otimes e)+t\,n\otimes n.
$$

The compatible geometry has $\nabla\theta=\kappa e$ with $\kappa=\theta_{,1}$, so $\nabla\cdot e=0$, $\nabla\cdot n=-\kappa$, $(e\cdot\nabla)e=\kappa n$ and $(n\cdot\nabla)e=0$. Resolving $\nabla\cdot\sigma=0$ along the two directions gives

$$
e\cdot\nabla s=2\kappa h-n\cdot\nabla h,\qquad n\cdot\nabla t-\kappa t=-e\cdot\nabla h-\kappa s.
$$

The [triangular equilibrium construction for inextensible-fibre plane strain](../../../../../triangular-equilibrium-construction-for-inextensible-fibre-plane-strain.md) now determines $s$ by integration along fibres and then $t$ along transverse curves. Thus any regular compatible deformation has a local zero-body-force stress construction once the shear law and suitable boundary integration data are supplied. There is no additional constitutive normal-stress law to specify: the two normal components are fixed by [force balance](../../../../../force-balance.md) and boundary [tractions](../../../../../traction.md). This does not assert that arbitrary separately prescribed boundary tractions can accompany an arbitrary deformation.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 76](../../paper-76-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
