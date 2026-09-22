<h1 id="6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For conserved nonrelativistic [dark matter](../../../../dark-matter.md) and [radiation](../../../../radiation.md), $\rho_{\rm DM}\propto a^{-3}$ and $\rho_\gamma\propto a^{-4}$, so $y=\rho_{\rm DM}/\rho_\gamma=a/a_{\rm eq}$ obeys $\dot y=yH$. Denote differentiation with respect to $y$ by a prime. Then

$$
\dot\delta=yH\delta',\qquad
\ddot\delta=y^2H^2\delta''+y(\dot H+H^2)\delta'.
$$

The supplied [Friedmann equations](../../../../friedmann-equations.md) imply

$$
\frac{\dot H}{H^2}=-\frac{4+3y}{2(1+y)},\qquad
\frac{4\pi G\rho_{\rm DM}}{H^2}=\frac{3y}{2(1+y)}.
$$

Substitution in the linear growth equation and division by $y^2H^2$ give the [Mészáros equation](../../../../meszaros-equation.md)

$$
\boxed{\delta''+\frac{2+3y}{2y(1+y)}\delta'-\frac{3}{2y(1+y)}\delta=0.}
$$

For $D_1=1+3y/2$, $D_1'=3/2$ and $D_1''=0$, making the two remaining terms cancel exactly. For [reduction of order](../../../../reduction-of-order.md), put $\delta=fD_1$ and $P=(2+3y)/[2y(1+y)]=1/y+1/[2(1+y)]$. The equation reduces to $f''+(2D_1'/D_1+P)f'=0$, whence

$$
f'=\frac{C}{y\sqrt{1+y}(1+3y/2)^2}.
$$

Using the supplied antiderivative and reversing an irrelevant overall sign gives the independent solution

$$
\boxed{D_2(y)=\left(1+\frac32y\right)\ln\frac{\sqrt{1+y}+1}{\sqrt{1+y}-1}-3\sqrt{1+y},\qquad
\delta=A_1D_1+A_2D_2.}
$$

Its [Wronskian](../../../../wronskian.md) is $D_1D_2'-D_1'D_2=-1/[y\sqrt{1+y}]\ne0$. The asymptotic expansions are

$$
\begin{array}{c|cc}
&D_1&D_2\\ \hline
y\ll1&1+3y/2&\ln(4/y)-3+O(y\ln(1/y))\\
y\gg1&3y/2+1&\frac4{15}y^{-3/2}+O(y^{-5/2})
\end{array}
$$

Thus subhorizon [dark matter](../../../../dark-matter.md) during [radiation domination](../../../../radiation-domination.md) has constant and logarithmic modes, rather than the superhorizon $a^2$ growth of [b](../b.md). A combination with negative $A_2$ supplies positive logarithmic growth. During [matter domination](../../../../matter-domination.md), the growing mode is proportional to $a$, agreeing with [b](../b.md), while the second mode decays as $a^{-3/2}$. These results neglect subhorizon radiation clustering; the [Mészáros equation](../../../../meszaros-equation.md) is the approximation stated in the question, not a full photon–matter perturbation system through horizon entry.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [6](../../6.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
