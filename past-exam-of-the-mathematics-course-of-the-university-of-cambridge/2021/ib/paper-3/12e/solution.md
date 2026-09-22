<h1 id="12e/solution">Solution</h1>

↑ **Parent:** [12E](../12e.md)

For a smooth curve $\gamma(t)$ on a [Riemannian surface](../../../../../riemannian-surface.md), its [energy of a curve](../../../../../energy-of-a-curve.md) is

$$
\boxed{\mathcal E(\gamma)=\frac12\int_0^1
\langle\dot\gamma,\dot\gamma\rangle\,dt}.
$$

Choose a local parameterization $\mathbf X(u,v)$ and write $\gamma(t)=\mathbf X(u(t),v(t))$. With coefficients of the [first fundamental form](../../../../../first-fundamental-form.md)

$$
E=\mathbf X_u\mathbin{\cdot}\mathbf X_u,\qquad
F=\mathbf X_u\mathbin{\cdot}\mathbf X_v,\qquad
G=\mathbf X_v\mathbin{\cdot}\mathbf X_v,
$$

the Lagrangian is

$$
L=\frac12(E\dot u^2+2F\dot u\dot v+G\dot v^2).
$$

The [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md) are equivalently

$$
\begin{aligned}
0={}&E\ddot u+F\ddot v
+(\mathbf X_{uu}\mathbin{\cdot}\mathbf X_u)\dot u^2
+2(\mathbf X_{uv}\mathbin{\cdot}\mathbf X_u)\dot u\dot v
+(\mathbf X_{vv}\mathbin{\cdot}\mathbf X_u)\dot v^2,\\
0={}&F\ddot u+G\ddot v
+(\mathbf X_{uu}\mathbin{\cdot}\mathbf X_v)\dot u^2
+2(\mathbf X_{uv}\mathbin{\cdot}\mathbf X_v)\dot u\dot v
+(\mathbf X_{vv}\mathbin{\cdot}\mathbf X_v)\dot v^2.
\end{aligned}
$$

After multiplying by the inverse metric these become the [geodesic equation](../../../../../geodesic-equation.md)

$$
\ddot q^k+\Gamma^k_{ij}\dot q^i\dot q^j=0,
$$

where the [Christoffel symbols](../../../../../christoffel-symbol.md) are determined by $E,F,G$.

If a straight line segment lies in the surface, parameterize it by

$$
\gamma(t)=P+t(Q-P).
$$

Then $\ddot\gamma=0$, so its acceleration has zero tangential component. The two displayed equations hold directly, and the segment is a geodesic.

For the one-sheeted [hyperboloid](../../../../../hyperboloid.md)

$$
H=\{(x,y,z):x^2+y^2-z^2=1\},
$$

put

$$
\rho_0=\sqrt{x_0^2+y_0^2}=\sqrt{1+z_0^2},\qquad
e_r=\frac1{\rho_0}(x_0,y_0,0),\qquad
e_\theta=\frac1{\rho_0}(-y_0,x_0,0).
$$

Two distinct ruling lines through $P$ are

$$
\boxed{\gamma_\pm(t)=P+t(z_0e_r\pm e_\theta+\rho_0e_z)}.
$$

Indeed, the direction $d_\pm$ satisfies

$$
x_0d_x+y_0d_y-z_0d_z=0,
\qquad
d_x^2+d_y^2-d_z^2=0,
$$

so substitution shows that every point of the line lies in $H$. These are geodesics by the straight-line argument.

A third geodesic is the meridian through $P$. Choose $s_0$ with $\sinh s_0=z_0$; then

$$
\boxed{\gamma_m(t)=\cosh(t+s_0)e_r+\sinh(t+s_0)e_z}.
$$

Its acceleration is $\gamma_m$, which is normal to $H$, so it is a geodesic. If $z_0\ne0$, these give the required three distinct subsets.

If $z_0=0$, there is also the equatorial circle. Writing $P=(\cos\theta_0,\sin\theta_0,0)$,

$$
\boxed{\gamma_e(t)=(\cos(t+\theta_0),\sin(t+\theta_0),0)}.
$$

Its acceleration is normal to $H$ along $z=0$, so it is a fourth geodesic distinct from the meridian and the two rulings.

Finally, write $\rho=\sqrt{x^2+y^2}=\sqrt{1+z^2}$. [Clairaut's relation](../../../../../clairaut-first-integral-for-a-surface-of-revolution.md) gives the conserved quantity

$$
c=\rho\sin\psi.
$$

Choose initial data in $z>0$ with

$$
1<c<\rho(0).
$$

Since $|\sin\psi|\leq1$, every point of the resulting geodesic satisfies $\rho\geq c$, and therefore

$$
z^2=\rho^2-1\geq c^2-1>0.
$$

Continuity keeps the geodesic in the component $z>0$, and the stated completeness assumption defines it for every real time. The continuum of choices of $c$ supplies infinitely many such geodesics.

## ↑ Ancestors (10)

1. [12E](../12e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
