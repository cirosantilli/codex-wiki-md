<h1 id="h/h2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $r=(x_1,x_2,x_3)^T$ for position relative to the [centroid](../../../../../centroid.md). The [inertia tensor](../../../../../inertia-tensor.md) there is

$$
\boxed{(J_G)_{ij}=\int_A\rho\bigl(|r|^2\delta_{ij}-x_ix_j\bigr)\,dV.}
$$

In particular its diagonal entries integrate the squares of distances from the corresponding axes, and its off-diagonal entries are the negative products of coordinates.

Insert $\mathbf v_Q=\mathbf v_G+\boldsymbol\omega\times r$ into $T=\tfrac12\int_A\rho|\mathbf v_Q|^2\,dV$. The cross term vanishes because $\int_A\rho r\,dV=0$. Using $|\boldsymbol\omega\times r|^2=|\boldsymbol\omega|^2|r|^2-(\boldsymbol\omega\cdot r)^2$ gives

$$
\boxed{T=\frac12m|\mathbf v_G|^2+\frac12\boldsymbol\omega^TJ_G\boldsymbol\omega.}
$$

If $a$ is the [vector](../../../../../vector.md) from $G$ to $O$, positions relative to $O$ are $r-a$. Expanding the defining tensor [integral](../../../../../integral-split.md) with this [substitution](../../../../../substitution-algebra.md) again removes the terms [linear](../../../../../linearity.md) in $r$. Thus the tensor [parallel axis theorem](../../../../../parallel-axis-theorem.md) is

$$
\boxed{J_O=J_G+m\bigl(|a|^2I-aa^T\bigr),\quad (J_O)_{ij}=(J_G)_{ij}+m(|a|^2\delta_{ij}-a_ia_j).}
$$

Since $O$ is fixed, $\mathbf v_G=\boldsymbol\omega\times(-a)$, so $m|\mathbf v_G|^2=m\boldsymbol\omega^T(|a|^2I-aa^T)\boldsymbol\omega$. [Substitution](../../../../../substitution-algebra.md) into the [energy](../../../../../energy-split.md) decomposition yields

$$
\boxed{T=\frac12\boldsymbol\omega^TJ_O\boldsymbol\omega.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [H2](../../h2.md)
3. [H](../../../h.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
