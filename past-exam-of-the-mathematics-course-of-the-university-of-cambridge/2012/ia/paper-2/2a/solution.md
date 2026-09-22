<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

A constant orbit is a [fixed point](../../../../../fixed-point.md) of $F(u)=u(1+u)/2$. Solving $F(u)=u$ gives $u(u-1)=0$, hence

$$
\boxed{u_n\equiv0\quad\text{and}\quad u_n\equiv1}.
$$

For [fixed point stability for an iteration](../../../../../fixed-point-stability-for-an-iteration.md), perturb a fixed point $u_*$ by $v_n$. Its local evolution is $v_{n+1}=F'(u_*)v_n+O(v_n^2)$, where $F'(u)=u+1/2$. At zero, $F'(0)=1/2$, so perturbations contract: **zero is locally asymptotically stable**. For example, if $|u|\leq r<1$, then $|F(u)|\leq(1+r)|u|/2$; this gives an invariant neighborhood and geometric convergence to zero.

At one, $F'(1)=3/2$, so perturbations expand: **one is unstable**. More explicitly, putting $u_n=1+v_n$ gives $v_{n+1}=3v_n/2+v_n^2/2$, whose magnitude increases while a nonzero perturbation remains sufficiently small. The derivative test concerns local stability; it does not assert attraction from every real initial value.

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
