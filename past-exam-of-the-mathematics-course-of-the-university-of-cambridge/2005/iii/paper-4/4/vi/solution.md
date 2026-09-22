<h1 id="4/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

Let every [root](../../../../../../root-of-a-root-system.md) have squared length $L$. Since $r+s$ is a root, $L=\|r+s\|^2=2L+2(r,s)$, hence $(r,s)=-L/2$. In particular the roots are independent. The potential higher sums satisfy

$$
\|2r+s\|^2=\|r+2s\|^2=3L,
$$

so neither is a root. The [root-space decomposition](../../../../../../root-space-decomposition.md) therefore gives $[e_r,e_{r+s}]=[e_s,e_{r+s}]=0$.

Set $A=t\operatorname{ad}e_r$, $B=u\operatorname{ad}e_s$ and $C=[A,B]=tuN_{r,s}\operatorname{ad}e_{r+s}$. Part (iv) shows $[A,C]=[B,C]=0$. To compute the sign, differentiate $F(v)=e^{-vB}Ae^{vB}$:

$$
F'(v)=e^{-vB}[A,B]e^{vB}=C,\qquad F(0)=A.
$$

Thus $e^{-B}Ae^B=A+C$. Conjugating the [matrix exponential](../../../../../../matrix-exponential.md), and then using the commutation of $A,C$, gives

$$
e^{-B}e^{-A}e^Be^A=e^{-A-C}e^A=e^{-C}.
$$

This proves the [central-commutator exponential identity](../../../../../../central-commutator-exponential-identity.md) in the required order, and consequently the [simply laced Chevalley commutator formula](../../../../../../simply-laced-chevalley-commutator-formula.md) is

$$
\boxed{x_s(u)^{-1}x_r(t)^{-1}x_s(u)x_r(t)=x_{r+s}(-N_{r,s}tu).}
$$

## ↑ Ancestors (11)

1. [Vi](../vi.md)
2. [4](../../4.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
