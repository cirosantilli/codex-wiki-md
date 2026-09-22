<h1 id="37b/solution">Solution</h1>

↑ **Parent:** [37B](../37b.md)

The outer fluid is at rest, so its pressure is constant; [boundary layer](../../../../../boundary-layer.md) normal balance gives no transverse pressure change, and the streamwise [pressure gradient](../../../../../pressure-gradient.md) is zero. The steady equations are $u_x+v_y=0$ and $uu_x+vu_y=\nu u_{yy}$. In conservative form $\partial_x(u^2)+\partial_y(uv)=\nu u_{yy}$. Integrating across the jet, with vanishing end contributions, proves $d[\rho\int u^2dy]/dx=0$. This is conserved [momentum flux](../../../../../momentum-flux.md). A control volume around the force source shows that its injected momentum per unit time and span is $F$, so **$M=F$**.

For width $b$ and velocity scale $U$, conservation gives $\rho U^2b\sim F$, while inertia-viscosity balance gives $U^2/x\sim\nu U/b^2$. Thus $b\sim(\rho\nu^2x^2/F)^{1/3}$, $U\sim[F^2/(\rho^2\nu x)]^{1/3}$ and [stream function](../../../../../stream-function.md) scale $Ub=(F\nu x/\rho)^{1/3}$. Put $\psi=Cx^{1/3}f(\eta)$, $\eta=Dyx^{-2/3}$, with the constants in the question. Then

$$
u=CDx^{-1/3}f',\qquad v=-\frac C3x^{-2/3}(f-2\eta f').
$$

Direct differentiation gives $uu_x+vu_y=-(C^2D^2/3)x^{-5/3}[(f\prime)^2+ff\prime\prime]$ and $\nu u_{yy}=\nu CD^3x^{-5/3}f\prime\prime\prime$. Since $C=\nu D$, their equality cancels the terms involving $\eta$ and gives

$$
\boxed{3f'''+(f')^2+ff''=0}.
$$

For $f=A\tanh(A\eta/6)$, differentiation verifies this equation directly. Moreover

$$
M=F\int_{-\infty}^\infty(f')^2d\eta
=F\frac{A^4}{36}\frac6A\frac43=F\frac{2A^3}{9}
$$

for $A>0$. Therefore momentum normalization fixes **$A=(9/2)^{1/3}$**. Independence of $x$ alone, as the last wording suggests, would not fix $A$; equality to the injected force does. Finally

$$
\boxed{Q(x)=\psi(x,\infty)-\psi(x,-\infty)=2A(F\nu x/\rho)^{1/3}}.
$$

[Entrainment](../../../../../fluid-entrainment.md) draws ambient fluid into the widening jet, so volume flux grows while [momentum flux](../../../../../momentum-flux.md) remains constant. These are the [laminar plane jet from a line force](../../../../../laminar-plane-jet-from-a-line-force.md) scalings.

## ↑ Ancestors (10)

1. [37B](../37b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
