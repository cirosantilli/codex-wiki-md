# Dirichlet image kernel for the three-dimensional Helmholtz equation

↑ **Parent:** [Outgoing Green function for the three-dimensional Helmholtz equation](outgoing-green-function-for-the-three-dimensional-helmholtz-equation.md)

For the upper half-space and the sign convention $(\Delta+k^2)G_D=\delta_{r'}$, reflect the source $r'=(x',y',z')$ to $r'^*=(x',y',-z')$ and use the displayed difference. This is the negative of the conventional outgoing kernel, whose source sign is $-\delta$. The [method of images](method-of-images.md) makes the [Dirichlet boundary condition](dirichlet-boundary-condition.md) zero on the plane. With $R=|r'-r|$ and $\cos\theta=z'/R$, its outward normal derivative there is

$$
\boxed{\partial_nG_D=-\frac{ik}{2\pi}\frac{e^{ikR}}R\left(1+\frac{i}{kR}\right)\cos\theta.}
$$

The outward [unit normal](unit-normal.md) is $-e_z$. Differentiating $e^{ikR}/R$ gives $e^{ikR}(ik/R-1/R^2)$; the real and reflected source contributions add in the normal derivative. [Green's second identity](green-second-identity.md) therefore expresses a solution of the [Helmholtz equation](helmholtz-equation.md) as $\phi(r')=\int_{z=0}\phi(r)\partial_nG_D(r,r')\,dS$ when the boundary term at infinity vanishes. Suitable decay or compatible outgoing [Sommerfeld radiation conditions](sommerfeld-radiation-condition.md) are needed; vanishing at infinity without further control is not a general uniqueness condition for a real-frequency Helmholtz problem.

## ↑ Ancestors (7)

1. [Outgoing Green function for the three-dimensional Helmholtz equation](outgoing-green-function-for-the-three-dimensional-helmholtz-equation.md)
2. [Helmholtz equation](helmholtz-equation.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/3/ii/b/solution.md)
