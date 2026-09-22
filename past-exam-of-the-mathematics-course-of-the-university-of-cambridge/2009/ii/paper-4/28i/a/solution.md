<h1 id="28i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Maximize $y(1)$. Along the positive-$y$ trajectory use [Hamiltonian of an optimal-control problem](../../../../../../hamiltonian-of-an-optimal-control-problem.md) $H=\sqrt y(pu+qv)$. The terminal [costate](../../../../../../costate.md) is $(p(1),q(1))=(0,1)$, and

$$
\dot p=0,\qquad\dot q=-\frac{pu+qv}{2\sqrt y}.
$$

Thus $p=0$. Maximizing over $u^2+v^2=1$ gives $u=0,v=1$ as long as $q>0$. The state equation integrates to $\sqrt{y(t)}=1/\sqrt2+t/2$, and the adjoint equation gives $q(t)=\sqrt{y(1)/y(t)}>0$, validating the maximization. Hence

$$
\boxed{u(t)=0,\quad v(t)=1,\quad x(t)=0,\quad y(t)=\left(\frac1{\sqrt2}+\frac t2\right)^2.}
$$

This is globally optimal, not just an extremal: whenever $y>0$, $d\sqrt y/dt=v/2\le1/2$. If a competitor reaches $y=0$ and later becomes positive, apply that bound after its last zero; it has even less remaining time to attain a positive terminal height. A negative terminal height cannot improve this positive maximum. Therefore the minimum objective is $\boxed{-y(1)=-(1/\sqrt2+1/2)^2}$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28I](../../28i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
