<h1 id="4/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Divide the equilibrium equation by $q>0$ to get $bq^2-q+a=0$. Hence both positive branches, when $0<4ab<1$, are

$$
q_\pm=\frac{1\pm\sqrt{1-4ab}}{2b}=\frac{C_uSL_u}{2}\left[1\pm\sqrt{1-4\frac{L_\rho C_\rho^2}{L_uC_u^2}\mathrm{Ri}}\right].
$$

At equilibrium, $\mathrm{Ri}_f=a/q=1-bq$. Therefore the larger-speed branch $q_+$ gives the **printed flux Richardson number**

$$
\boxed{\mathrm{Ri}_f=\frac12\left[1-\sqrt{1-4\frac{L_\rho C_\rho^2}{L_uC_u^2}\mathrm{Ri}}\right],}
$$

while the smaller-speed branch gives the same formula with a plus sign before the square root. Solving the quadratic alone does not discard that second branch.

The larger-speed branch is selected by local kinetic-energy stability. If the same closures are used in the local energy evolution, $\tfrac12d(q^2)/dt=\mathcal P-B-\epsilon$. For $q>0$, divide by $q$ to obtain

$$
\dot q=C_uSq-C_\rho^2L_\rho N^2-q^2/L_u.
$$

Its linearization at $q_\pm$ has derivative $C_uS-2q_\pm/L_u=\mp C_uS\sqrt{1-4ab}$. The upper branch is therefore stable and the lower unstable in this local closure model.

The discriminant gives the **critical gradient Richardson number**

$$
\boxed{\mathrm{Ri}_c=\frac{L_uC_u^2}{4L_\rho C_\rho^2}.}
$$

At criticality the branches meet and $\mathrm{Ri}_f=1/2$. At zero stratification the stable positive solution is $q=C_uSL_u$ with $\mathrm{Ri}_f=0$; the lower algebraic root is $q=0$. This closure-dependent critical value is not automatically the inviscid $1/4$ criterion of the [Miles–Howard theorem](../../../../../../miles-howard-theorem.md).

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [4](../../4.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
