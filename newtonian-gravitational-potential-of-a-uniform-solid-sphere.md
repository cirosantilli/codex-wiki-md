# Newtonian gravitational potential of a uniform solid sphere

↑ **Parent:** [Newtonian gravitational potential](newtonian-gravitational-potential.md)

For radius $R$, constant [mass density](density.md) $\rho$ and $M=4\pi\rho R^3/3$, normalize the [Newtonian gravitational potential](newtonian-gravitational-potential.md) to zero at infinity. Then

$$
\boxed{\Phi(r)=\begin{cases}-\dfrac{GM}{2R^3}(3R^2-r^2),&0\leq r\leq R,\\-GM/r,&r\geq R.\end{cases}}
$$

By the [spherical shell theorem](spherical-shell-theorem.md), each spherical shell contributes the potential of a point mass outside it and a constant inside it. Summing inner and outer shells gives $\Phi(r)=-4\pi G\rho[r^2/3+(R^2-r^2)/2]$ inside. Equivalently, angular integration of the free-space [Green function of the Laplacian](green-function-of-the-laplacian.md) gives $\int_{-1}^1(r^2+r'^2-2rr'\mu)^{-1/2}d\mu=[r+r'-|r-r'|]/(rr')$. The resulting radial integral has the same value.

The potential and its first radial derivative are continuous at $R$. The interior [gravitational acceleration](gravitational-acceleration.md) is $-\nabla\Phi=-(GM/R^3)\mathbf r$, and $\nabla^2\Phi=4\pi G\rho$. At the centre $\Phi(0)=-3GM/(2R)$ while its gradient vanishes.

## ↑ Ancestors (7)

1. [Newtonian gravitational potential](newtonian-gravitational-potential.md)
2. [Newtonian gravitational field](newtonian-gravitational-field.md)
3. [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation-split.md)
4. [Classical mechanics](classical-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2/3/ii/solution.md)
