<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

All requester indices in the following expressions are interpreted [modulo](../../../../../modulo-operation.md) four. Let $h_{\ell,j}$ mean that requester $j$ is the first asserted request after last recipient $\ell$:

$$
h_{\ell,\ell+d}=r_{\ell+d}\land\bigwedge_{t=1}^{d-1}\neg r_{\ell+t},\qquad d=1,2,3,4.
$$

An empty [logical conjunction](../../../../../logical-conjunction.md) is true. Decode the remembered index and combine the four priority orders:

$$
w_j=\bigvee_{\ell=0}^3([L=\ell]\land h_{\ell,j}),\qquad H=\bigvee_{j=0}^3r_j.
$$

Exactly one $w_j$ is high when any request is high. Write $L$ as bits $L_1L_0$. The [next-state function](../../../../../next-state-function.md) and [Moore machine](../../../../../moore-machine.md) outputs are

$$
\boxed{\begin{aligned}
V^+&=H,\\
L_1^+&=(\neg H\land L_1)\lor w_2\lor w_3,\\
L_0^+&=(\neg H\land L_0)\lor w_1\lor w_3,\\
g_j&=V\land[L=j].
\end{aligned}}
$$

Thus an idle step preserves the priority memory. The $w_j$ are combinational selection signals, not the current-cycle grants: exposing them directly as outputs would change the design into a [Mealy machine](../../../../../mealy-machine.md). If a requester remains continuously asserted, each intervening successful grant advances the circular order, so it receives service after at most four grant decisions.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
