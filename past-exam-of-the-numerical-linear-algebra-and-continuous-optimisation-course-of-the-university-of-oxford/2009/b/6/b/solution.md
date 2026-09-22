<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [active constraint set](../../../../../active-constraint-set.md) is $\boxed{\mathcal A(x)=\{j:c_j(x)=0\}}$, and the [linearized tangent cone](../../../../../linearized-tangent-cone.md) is

$$
\boxed{F(x)=\{d:\nabla c_j(x)^Td\geq0\text{ for }j\in\mathcal A(x)\}.}
$$

Differentiating each active feasibility inequality along a tangent sequence gives $T_\Omega(x)\subseteq F(x)$. A sufficient condition for equality is the [linear independence constraint qualification](../../../../../linear-independence-constraint-qualification.md): the active constraint gradients are linearly independent. The weaker [Mangasarian–Fromovitz constraint qualification](../../../../../mangasarian-fromovitz-constraint-qualification.md) also suffices in this inequality-only setting.

Under the stated independence condition, the necessary first-order conditions become the [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md): there are multipliers $\lambda_j$ with

$$
\boxed{\nabla f(x_*)-\sum_j\lambda_j\nabla c_j(x_*)=0,\quad c_j(x_*)\geq0,\quad\lambda_j\geq0,\quad\lambda_jc_j(x_*)=0.}
$$

Use the allowed span assertion to write $\nabla f(x_*)=\sum_{j\in\mathcal A}\lambda_j\nabla c_j(x_*)$. Independence gives vectors $\varphi_i$ with $\nabla c_j(x_*)^T\varphi_i=\delta_{ji}$ for the active indices. Each $\varphi_i$ lies in $F=T_\Omega$, so part (a) gives $\lambda_i=\nabla f(x_*)^T\varphi_i\geq0$. Assign zero multipliers to inactive constraints. This proves all displayed conditions, including complementarity. Conversely, their stationarity and sign conditions imply $\nabla f(x_*)^Td=\sum_{j\in\mathcal A}\lambda_j\nabla c_j(x_*)^Td\geq0$ for every $d\in F$. Thus they reformulate the first-order inequality; they do not alone prove a minimum for a nonconvex problem.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra and continuous optimisation course of the University of Oxford](../../../../../numerical-linear-algebra-and-continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
