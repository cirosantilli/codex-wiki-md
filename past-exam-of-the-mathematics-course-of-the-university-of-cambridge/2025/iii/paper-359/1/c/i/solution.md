<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The estimates from part b make $(u_m)$ bounded in

$$
L^\infty(0,T;H)\cap L^2(0,T;V),
$$

and $(\partial_tu_m)$ bounded in $L^2(0,T;V')$. Since the periodic embedding $V\Subset H$ is compact, the [Aubin-Lions lemma](../../../../../../../aubin-lions-lemma.md) supplies a subsequence such that

$$
u_m\rightharpoonup^*u
\quad\hbox{in }L^\infty(0,T;H),
$$



$$
u_m\rightharpoonup u
\quad\hbox{in }L^2(0,T;V),
\qquad
u_m\to u
\quad\hbox{in }L^2(0,T;H).
$$

The derivatives converge weakly in $L^2(0,T;V')$ to $\partial_tu$.

Because $P_NH$ is fixed and finite dimensional, strong convergence in $H$ implies

$$
P_Nu_m\to P_Nu
\quad\hbox{strongly in }L^2(0,T;V).
$$

Combining this with the uniform $L^\infty H$ and $L^2V$ bounds in the estimate from part a identifies the weak limit

$$
B(P_Nu_m,u_m)\rightharpoonup B(P_Nu,u)
\quad\hbox{in }L^2(0,T;V').
$$

Passing to the limit in the Galerkin identity gives

$$
\boxed{
\frac{du}{dt}+\nu Au+B(P_Nu,u)=0
\quad\hbox{in }L^2(0,T;V')}.
$$

The projected initial data converge to $u_0$ in $H$, so $u(0)=u_0$.

The [weak continuity from evolution-space bounds](../../../../../../../weak-continuity-from-evolution-space-bounds.md) gives

$$
\boxed{
u\in C([0,T];H_{\rm weak})
\cap L^\infty(0,T;H)
\cap L^2(0,T;V),
\qquad
u_t\in L^2(0,T;V')}.
$$

Since $T$ was arbitrary, this is a global weak solution of the [Navier-Stokes equation with spectrally truncated advection](../../../../../../../navier-stokes-equation-with-spectrally-truncated-advection.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 359](../../../../paper-359-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
