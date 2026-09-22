<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the index convention $[e_a,e_c]=C_a{}^b{}_c e_b$. For the left- and right-invariant coframes, the [Maurer-Cartan equations](../../../../../maurer-cartan-equation.md) are

$$
\boxed{d\lambda^b=-\frac12C_a{}^b{}_c\lambda^a\wedge\lambda^c,\qquad
d\rho^b=+\frac12C_a{}^b{}_c\rho^a\wedge\rho^c.}
$$

Their dual invariant vector fields satisfy

$$
\boxed{[L_a,L_c]=C_a{}^b{}_cL_b,\qquad
[R_a,R_c]=-C_a{}^b{}_cR_b,\qquad[L_a,R_c]=0.}
$$

For example, evaluating $d\lambda^b$ on two dual fields gives $-\lambda^b([L_a,L_c])$, since its invariant coefficient functions are constant. The opposite right-invariant bracket gives the other sign. The mixed bracket vanishes because left and right translations commute.

For a [semisimple Lie algebra](../../../../../semisimple-lie-algebra-split.md), the [Killing form](../../../../../killing-form.md) $B(X,Y)=\operatorname{Tr}(\operatorname{ad}X\operatorname{ad}Y)$ is nondegenerate. It is adjoint invariant: using $\operatorname{ad}[Z,X]=[\operatorname{ad}Z,\operatorname{ad}X]$ and cyclicity of trace gives

$$
B([Z,X],Y)+B(X,[Z,Y])=0.
$$

Group conjugation preserves the trace as well, so this is invariant under the full group adjoint action. Translation supplies a [bi-invariant pseudo-Riemannian metric](../../../../../bi-invariant-pseudo-riemannian-metric.md).

Lower the indicated structure index by $C_{abc}=B_{be}C_a{}^e{}_c$. Then

$$
C_{abc}=B(e_b,[e_a,e_c])=-B(e_a,[e_b,e_c]).
$$

This changes sign under exchange of $a,c$ by the bracket and under exchange of $a,b$ by invariance. Hence **$C_{abc}=C_{[abc]}$**.

Let $\eta(X,Y,Z)=B(X,[Y,Z])$ at the identity and extend it as a [left-invariant differential form](../../../../../left-invariant-differential-form.md). Its value is adjoint invariant, so the extended form is also right-invariant. The three-form in the question is $-\eta$ with the index-lowering convention just specified, an irrelevant overall sign for these properties. To prove closedness rather than only invariance, apply the [exterior derivative](../../../../../exterior-derivative.md) on four left-invariant fields. Its six bracket terms combine by invariance into

$$
\begin{aligned}
d\eta(W,X,Y,Z)
&=-2\bigl[B([W,X],[Y,Z])-B([W,Y],[X,Z])+B([W,Z],[X,Y])\bigr]\\
&=-2B\bigl(W,[X,[Y,Z]]+[Y,[Z,X]]+[Z,[X,Y]]\bigr)=0.
\end{aligned}
$$

The final equality is the [Jacobi identity](../../../../../jacobi-identity.md). Therefore the [Cartan three-form](../../../../../cartan-three-form.md)

$$
\boxed{\frac1{3!}C_{abc}\lambda^a\wedge\lambda^b\wedge\lambda^c}
$$

is both **bi-invariant and closed**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 74](../../paper-74-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
