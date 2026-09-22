<h1 id="28k/solution">Solution</h1>

↑ **Parent:** [28K](../28k.md)

The [Pontryagin maximum principle](../../../../../pontryagin-maximum-principle.md) addresses optimization of an integral running reward, possibly with terminal reward, subject to a controlled differential equation, admissible control constraints and prescribed endpoint conditions. For a normal maximization problem $\dot x=f(t,x,u)$ with running reward $L$, the [Hamiltonian](../../../../../hamiltonian.md) is $H=L+\lambda f$; the [optimal control](../../../../../optimal-control.md) maximizes it pointwise, and the adjoint satisfies $\dot\lambda=-H_x$ with the appropriate terminal transversality condition. State constraints require additional care when active.

Assume $p>0$ and $x(0)>0$. Here

$$
\boxed{H(x,u,\lambda)=(p-\lambda)u-u^2/x.}
$$

The terminal stock is free and has no salvage reward, so an optimum with positive terminal stock has $\lambda(T)=0$. For $x>0$, maximization over $u\ge0$ gives $u=x(p-\lambda)/2$ whenever $p-\lambda>0$. Then

$$
\dot\lambda=-u^2/x^2=-\tfrac14(p-\lambda)^2.
$$

Set $v=p-\lambda$, so $\dot v=v^2/4$ and $v(T)=p$. Integrating gives

$$
\boxed{\lambda(t)=p-\frac1{1/p+(T-t)/4},\qquad
\dot x=-\frac{2px}{4+p(T-t)}.}
$$

The resulting $p-\lambda$ is positive throughout, validating the interior control formula. Integrating the state equation yields

$$
\boxed{x(t)=x(0)\left(\frac{4+p(T-t)}{4+pT}\right)^2,\qquad
x(T)=\frac{16x(0)}{(4+pT)^2}.}
$$

The state remains positive, so its nonnegativity constraint is inactive and the terminal condition is consistent. The reward $pu-u^2/x$ is jointly concave in $(x,u)$ and the dynamics are linear, giving sufficiency of this solution. Alternatively the value function $V(t,x)=\lambda(t)x$ satisfies the [Hamilton-Jacobi-Bellman equation](../../../../../hamilton-jacobi-bellman-equation.md) with this maximizing control. At zero price the [optimal control](../../../../../optimal-control.md) is zero, obtained by a continuous $p\downarrow0$ limit; zero initial stock also gives zero extraction.

## ↑ Ancestors (10)

1. [28K](../28k.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
