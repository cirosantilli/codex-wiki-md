<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Odd elements of a [Grassmann algebra](../../../../../grassmann-algebra.md) anticommute, and in particular $\psi_i^2=0$. For variations with fixed endpoints, move each odd variation to the left before applying [integration by parts](../../../../../integration-by-parts.md). For example,

$$
\delta(\psi\dot\psi)=\delta\psi\dot\psi+\psi\delta\dot\psi
\quad\Longrightarrow\quad
\delta\int\psi\dot\psi\,dt=2\int\delta\psi\dot\psi\,dt.
$$

The interaction varies as $\delta_{\psi_1}(\psi_1\psi_2)=\delta\psi_1\psi_2$ and $\delta_{\psi_2}(\psi_1\psi_2)=-\delta\psi_2\psi_1$. Thus variation of the [action](../../../../../action.md) gives the [Euler-Lagrange equations](../../../../../euler-lagrange-equation.md)

$$
\boxed{\ddot x=UU'+U''\psi_1\psi_2,\qquad \dot\psi_1=U'\psi_2,\qquad \dot\psi_2=U'\psi_1.}
$$

All products of $U$ and its derivatives commute with the odd variables. These signs are essential for this variant of [Grassmann-valued classical supersymmetric mechanics](../../../../../grassmann-valued-classical-supersymmetric-mechanics.md).

The fermion bilinear is constant along a solution:

$$
\frac{d}{dt}(\psi_1\psi_2)=\dot\psi_1\psi_2+\psi_1\dot\psi_2=U'(\psi_2^2+\psi_1^2)=0.
$$

For the [energy](../../../../../energy.md), direct differentiation now gives

$$
\dot E=\dot x(\ddot x-UU'-U''\psi_1\psi_2)-U'\frac{d}{dt}(\psi_1\psi_2)=0.
$$

Similarly the given [supercharge](../../../../../supersymmetry-generator.md), denoted $Q_1$, satisfies

$$
\begin{aligned}
\dot Q_1&=\ddot x\psi_1+\dot x\dot\psi_1-U'\dot x\psi_2-U\dot\psi_2\\
&=(\ddot x-UU')\psi_1=U''\psi_1\psi_2\psi_1=0.
\end{aligned}
$$

A second conserved [supercharge](../../../../../supersymmetry-generator.md) is

$$
\boxed{Q_2=\dot x\psi_2-U\psi_1,}
$$

since $\dot Q_2=(\ddot x-UU')\psi_2=U''\psi_1\psi_2\psi_2=0$. The two charges are independent functions on the unrestricted [phase space](../../../../../phase-space.md): their coefficient matrix on $(\psi_1,\psi_2)$ has [determinant](../../../../../determinant.md) $\dot x^2-U^2$, and is invertible wherever its even body is nonzero. They can become dependent on a restricted family of trajectories.

Under $\dot x=U$ and $\psi_2=-\psi_1$, the bilinear $\psi_1\psi_2$ vanishes. Differentiating the first-order equation gives $\ddot x=U'\dot x=UU'$, which is the bosonic [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md). The first fermionic equation becomes $\dot\psi_1=-U'\psi_1$; differentiating $\psi_2=-\psi_1$ gives $\dot\psi_2=U'\psi_1$, so the second fermionic equation holds too. This establishes the [first-order zero-energy solution in Grassmann supersymmetric mechanics](../../../../../first-order-zero-energy-solution-in-grassmann-supersymmetric-mechanics.md) without imposing an additional equation.

Let $x_0=x(0)$ and $\psi_{10}=\psi_1(0)$. For $U=1+cx$ and $c\ne0$, solve $d(x+1/c)/dt=c(x+1/c)$ and $\dot\psi_1=-c\psi_1$ to obtain

$$
\boxed{x(t)=e^{ct}x_0+\frac{e^{ct}-1}{c},\qquad \psi_1(t)=e^{-ct}\psi_{10},\qquad \psi_2(t)=-e^{-ct}\psi_{10}.}
$$

For $c=0$, the nonsingular limiting answer is $\boxed{x(t)=x_0+t,\ \psi_1(t)=\psi_{10},\ \psi_2(t)=-\psi_{10}}$. These formulas also hold for even initial positions in the [Grassmann algebra](../../../../../grassmann-algebra.md) by ordinary polynomial evaluation. Finally, $U(x(t))=(1+cx_0)e^{ct}$, so the conserved quantities are

$$
\boxed{E=0,\qquad Q_1=2(1+cx_0)\psi_{10},\qquad Q_2=-2(1+cx_0)\psi_{10}.}
$$

The individual odd [supercharges](../../../../../supersymmetry-generator.md) generally do not vanish, although their sum vanishes on this restricted solution.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
