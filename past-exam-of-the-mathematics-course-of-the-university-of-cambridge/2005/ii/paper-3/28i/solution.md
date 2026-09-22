<h1 id="28i/solution">Solution</h1>

↑ **Parent:** [28I](../28i.md)

Interpret unit-intensity Gaussian white noise as $dW_t/dt$. Differentiating $z=x+(T-t)y$ cancels the two $y\,dt$ terms and gives

$$
\boxed{dz=(T-t)u\,dt+(T-t)dW_t,\qquad z(T)=x(T).}
$$

The cost is terminal $z(T)^2$ plus the same running $u^2$. Write $h=T-t$ and guess the value $V(t,z)=P(t)z^2+C(t)$. The [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md) is

$$
V_t+\tfrac12h^2V_{zz}+\min_u(u^2+huV_z)=0,\qquad V(T,z)=z^2.
$$

Completing the square gives $u_*=-hPz$. Equating powers yields $P'=h^2P^2$, $C'=-h^2P$, with $P(T)=1,C(T)=0$. Integration gives

$$
\boxed{P(t)=\frac1{1+(T-t)^3/3},\quad C(t)=\log[1+(T-t)^3/3],\quad
u_*=-\frac{(T-t)z}{1+(T-t)^3/3}.}
$$

Indeed $V_t+\mathcal L^uV+u^2=(u+hPz)^2\geq0$, and the Itô verification identity attains equality at this control. This proves optimality for admissible controls of finite expected quadratic cost. The additive noise changes only $C$, not the feedback gain, so **this is certainty-equivalence control**. A different constant noise intensity multiplies $C$ but leaves the control unchanged, as in the [terminal-position reduction of double-integrator control](../../../../../terminal-position-reduction-of-double-integrator-control.md).

## ↑ Ancestors (10)

1. [28I](../28i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
