<h1 id="35e/solution">Solution</h1>

↑ **Parent:** [35E](../35e.md)

First retain the question's units $c=1$. Insert the [retarded time](../../../../../retarded-time.md) [Dirac delta](../../../../../dirac-delta-function.md):

$$
\phi(t,x)=\frac1{4\pi\epsilon_0}\int d^3x'\,dt'\,
\frac{\rho(t',x')}{|x-x'|}\delta(t-t'-|x-x'|).
$$

For a [point charge](../../../../../point-charge.md), the spatial delta sets $x'=x_0(t')$. Put $R(t')=|x-x_0(t')|$, $\widehat R=(x-x_0)/R$ and $v=\dot x_0(t')$. The retarded root $t_*$ satisfies $t-t_*=R(t_*)$. The derivative of the delta's argument is $-1+\widehat R\cdot v$, so for a subluminal trajectory its absolute value is $1-\widehat R\cdot v$. Performing the time integral gives

$$
\boxed{\phi(t,x)=\frac q{4\pi\epsilon_0}\frac1{R_*-v_*\cdot\mathbf R_*}},\qquad
\mathbf R_*=x-x_0(t_*),\quad R_*=|\mathbf R_*|.
$$

All quantities in the denominator are evaluated at the [retarded time](../../../../../retarded-time.md). The retarded [vector potential](../../../../../vector-potential.md) uses current $j=qv\delta^{(3)}(x'-x_0)$ and the same [Jacobian determinant](../../../../../jacobian-determinant.md), giving

$$
\boxed{\mathbf A(t,x)=\frac{\mu_0q}{4\pi}\frac{v_*}{R_*-v_*\cdot\mathbf R_*}}\quad(c=1).
$$

Restoring physical $c$, the root is $t-t_*=R_*/c$, both denominators become $R_*-v_*\cdot\mathbf R_*/c$, and $\mu_0=1/(\epsilon_0c^2)$. Thus $\mathbf A=v_*\phi/c^2$. This is the [Liénard–Wiechert potential](../../../../../lienard-wiechert-potential.md); the [Jacobian determinant](../../../../../jacobian-determinant.md), rather than merely substituting retarded position into a static Coulomb formula, accounts for the velocity factor.

## ↑ Ancestors (10)

1. [35E](../35e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
