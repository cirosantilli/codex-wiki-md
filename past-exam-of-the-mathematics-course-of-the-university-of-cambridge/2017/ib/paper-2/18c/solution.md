<h1 id="18c/solution">Solution</h1>

↑ **Parent:** [18C](../18c.md)

Specify the [Minkowski metric](../../../../../minkowski-metric.md) convention $\eta_{\mu\nu}=\eta^{\mu\nu}=\operatorname{diag}(1,-1,-1,-1)$, with $x^0=ct$ and $\partial_0=c^{-1}\partial_t$. For the [electromagnetic four-potential](../../../../../electromagnetic-four-potential.md), $A_\mu=\eta_{\mu\nu}A^\nu=(\phi/c,-\mathbf A)$. The [electromagnetic field tensor](../../../../../electromagnetic-field-tensor.md) is

$$
F_{\mu\nu}=\partial_\mu A_\nu-\partial_\nu A_\mu,\qquad
F^{\mu\nu}=\eta^{\mu\rho}\eta^{\nu\sigma}F_{\rho\sigma}.
$$

Using $\mathbf E=-\nabla\phi-\partial_t\mathbf A$ and $\mathbf B=\nabla\times\mathbf A$, its two component matrices are

$$
\boxed{F_{\mu\nu}=\begin{pmatrix}
0&E_x/c&E_y/c&E_z/c\\
-E_x/c&0&-B_z&B_y\\
-E_y/c&B_z&0&-B_x\\
-E_z/c&-B_y&B_x&0
\end{pmatrix},\quad
F^{\mu\nu}=\begin{pmatrix}
0&-E_x/c&-E_y/c&-E_z/c\\
E_x/c&0&-B_z&B_y\\
E_y/c&B_z&0&-B_x\\
E_z/c&-B_y&B_x&0
\end{pmatrix}.}
$$

Changing metric/sign conventions changes the component convention, so stating it is necessary. Under a [Lorentz transformation](../../../../../lorentz-transformation.md), the tensor law is $F'^{\mu\nu}(x')=\Lambda^\mu{}_{\rho}\Lambda^\nu{}_{\sigma}F^{\rho\sigma}(x)$. For the stated [Lorentz boost](../../../../../lorentz-boost.md), put $\beta=v/c$ and $\gamma=(1-\beta^2)^{-1/2}$:

$$
\Lambda=\begin{pmatrix}\gamma&-\gamma\beta&0&0\\-\gamma\beta&\gamma&0&0\\0&0&1&0\\0&0&0&1\end{pmatrix}.
$$

Multiplication $F'=\Lambda F\Lambda^T$ gives, for example, $F'^{02}=-\gamma E_y/c+\gamma\beta B_z$ and $F'^{12}=-\gamma B_z+\gamma\beta E_y/c$. Reading off all entries proves [Lorentz transformation of electromagnetic fields](../../../../../lorentz-transformation-of-electromagnetic-fields.md):

$$
\boxed{\begin{aligned}
E'_x&=E_x,&E'_y&=\gamma(E_y-vB_z),&E'_z&=\gamma(E_z+vB_y),\\
B'_x&=B_x,&B'_y&=\gamma(B_y+vE_z/c^2),&B'_z&=\gamma(B_z-vE_y/c^2).
\end{aligned}}
$$

For the wire, the lab line charge is zero and the current is $I=nqu+(-nq)(-u)=2nqu$. At points off the wire, write $s^2=y^2+z^2>0$. [Gauss's law](../../../../../gauss-s-law.md) and [Ampère's law](../../../../../ampere-s-circuital-law.md) give

$$
\boxed{\mathbf E=0,\qquad\mathbf B=\frac{\mu_0I}{2\pi s^2}(0,-z,y)
=\frac{\mu_0nqu}{\pi s^2}(0,-z,y).}
$$

The boost leaves $y,z$ unchanged, so the field transformations give

$$
\boxed{\mathbf E'=-\frac{\gamma\mu_0nquv}{\pi(y^2+z^2)}(0,y,z).}
$$

Its physical source is the [relativistic charge density of counterstreaming beams](../../../../../relativistic-charge-density-of-counterstreaming-beams.md). Their boosted number densities are $n'_+=\gamma n(1-vu/c^2)$ and $n'_- =\gamma n(1+vu/c^2)$, by transforming each charge-current four-vector. Thus $\lambda'=q(n'_+-n'_-)=-2\gamma nquv/c^2=-\gamma vI/c^2$. A line charge has radial field $\lambda'(0,y,z)/(2\pi\epsilon_0s^2)$; using $\mu_0\epsilon_0c^2=1$ reproduces the boxed field. Oppositely moving populations contract differently under the boost, so neutrality in one frame does not imply neutrality in the other. The ideal wire's fields are singular on its axis.

## ↑ Ancestors (10)

1. [18C](../18c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
