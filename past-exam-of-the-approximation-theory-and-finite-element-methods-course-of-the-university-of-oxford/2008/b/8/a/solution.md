<h1 id="b/8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the full continuous piecewise linear space $V_h\subset H^1(0,1)$, including endpoint basis [functions](../../../../../function-split.md), because the [boundary conditions](../../../../../boundary-condition.md) are Neumann. Define

$$
a(w,v)=\int_0^1(w'v'+e^xwv).
$$

Choose $u_h^0$ as the $L^2$ projection of $u_0$ onto $V_h$. For each time step seek $u_h^{m+1}\in V_h$ with

$$
\boxed{\left(\frac{u_h^{m+1}-u_h^m}{\Delta t},v_h\right)
+a\left(\frac{u_h^{m+1}+u_h^m}{2},v_h\right)=0
\quad(v_h\in V_h).}
$$

This is the conforming [Crank-Nicolson method](../../../../../crank-nicolson-method.md). The reaction coefficient and the diffusion are both treated at the midpoint; integration by parts has removed the boundary flux through the homogeneous Neumann condition.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [8](../../8.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
