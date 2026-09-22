<h1 id="1/c/vi/solution">Solution</h1>

↑ **Parent:** [Vi](../vi.md)

The printed uniqueness assertion has an exceptional case at $n=4$. To locate it, use the two [double cosets](../../../../../../../double-coset.md)

$$
S_n=H\sqcup HtH,\qquad t=(n-1\ n).
$$

An $H$-bimodule-equivariant set map is determined by $u=\Phi(1)$ and $v=\Phi(t)$. Equivariance requires $u\in Z(H)$ and

$$
v\in C_H(S_{n-2}),
$$

because $H\cap tHt=S_{n-2}$ and $t$ commutes with this subgroup. These conditions are also sufficient: define $\Phi(h)=hu$ and $\Phi(hth')=hvh'$. Changing the double-coset expression only inserts an element of $S_{n-2}$, which commutes with $v$.

For $n\geq5$, the center of $H$ and this [centralizer](../../../../../../../centralizer.md) are both trivial. For the latter, a commuting permutation must fix the unique point outside $\{1,\ldots,n-2\}$ and lie in the center of $S_{n-2}$; that center is trivial when $n-2\geq3$. Therefore $u=v=1$, giving deletion. For $n=4$, however, $C_{S_3}(S_2)=\{1,(1\ 2)\}$. The choice

$$
\Phi(h)=h,\qquad \Phi(h(3\ 4)h')=h(1\ 2)h'
$$

is well defined and satisfies all the printed equivariance conditions, but sends $(3\ 4)$ to $(1\ 2)$ rather than to the identity. **Uniqueness holds for $n\geq5$; it is false at $n=4$ as printed.** Even requiring the map to restrict to the identity on $H$ does not remove this counterexample.

## ↑ Ancestors (12)

1. [Vi](../vi.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 103](../../../../paper-103-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
