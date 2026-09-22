<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [phase-space path integral](../../../../../../phase-space-path-integral.md) is defined as a limit of finite-dimensional integrals, not by assigning a classical derivative to every path. Choose $t_1=0<t_2<\cdots<t_{N+1}=T$, let $\Delta t_i=t_{i+1}-t_i$, and set $q_{N+1}=q_f$. On slice $i$ the precise prescription is

$$
\boxed{\dot q_i:=\frac{q_{i+1}-q_i}{\Delta t_i},\qquad
\int p\dot q\,dt\longrightarrow\sum_{i=1}^N p_i(q_{i+1}-q_i).}
$$

The remaining Hamiltonian term must have a compatible operator-ordering prescription. For example, evaluate $H$ at $(p_i,(q_{i+1}+q_i)/2)$ for midpoint/Weyl ordering. A prepoint prescription $H(p_i,q_i)$ defines a corresponding ordering instead. This choice matters for a general mixed $H(p,q)$; the separable kinetic-plus-potential Hamiltonian in the next part admits the usual Trotter prescription.

This is [time slicing of a phase-space path integral](../../../../../../time-slicing-of-a-phase-space-path-integral.md). Integrate the intermediate $q_i$ and the slice momenta and only then take $\max_i\Delta t_i\to0$. Typical paths of the [Euclidean path integral](../../../../../../euclidean-path-integral.md) need not be differentiable; the finite difference is the meaning of the printed $\dot q$. For a fixed-endpoint kernel the initial coordinate is fixed as well, whereas propagation of a [wavefunction](../../../../../../wave-function.md) includes an integral over that initial coordinate.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
