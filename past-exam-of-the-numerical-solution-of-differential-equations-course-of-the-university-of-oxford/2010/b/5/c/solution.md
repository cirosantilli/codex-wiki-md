<h1 id="b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The displayed estimate requires a nonnegative barrier. As printed, a counterexample is obtained with two interior nodes, each having row $L_hv_p=v_a-v_p$ to one boundary node. Set $e_a=0$, $e_p=1$, and $\phi_a=-1$, $\phi_p=-2$. Both interior rows have $|T_p|=1$ and $L_h\phi_p=1$. Put one node in each of $J_1,J_2$ and take $T=S=d_1=d_2=1$. Then the proposed right-hand side is $-1$ while $E=1$.

For the intended use, suppose $\phi_p\geq0$ and the stencil has the maximum principle established in part (a). Set $C=\max\{T/d_1,S/d_2\}$. On either subregion,

$$
L_h(\pm e+C\phi)\geq-|T_p|+Cd_i\geq0.
$$

At boundary nodes these functions equal $C\phi_a$. Hence

$$
\pm e_p\leq C\left(\max_a\phi_a-\phi_p\right)\leq C\max_a\phi_a,
$$

which proves the intended [discrete elliptic barrier](../../../../../discrete-elliptic-barrier.md) estimate

$$
\boxed{E\leq\max_{a\in J_{\partial\Omega}}\phi_a\max\{T/d_1,S/d_2\}.}
$$

For a normalized stencil with $L_h1=0$ and a sign-changing barrier, shifting it by its minimum gives the valid general replacement $E\leq C(\max_a\phi_a-\min_p\phi_p)$. The supplied barrier in part (d) is positive, so the printed estimate applies there without a sign problem.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
