<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the given [group homomorphism](../../../../group-homomorphism.md) $\varphi:H\to\operatorname{Aut}(N)$, the external [semidirect product](../../../../semidirect-product.md) has underlying [Cartesian product](../../../../cartesian-product.md) $N\times H$ and operation

$$
\boxed{(n,h)(m,k)=\bigl(n\varphi(h)(m),hk\bigr).}
$$

The notation $\operatorname{Aut}(N)$ denotes the [automorphism group](../../../../automorphism-group.md) of $N$. Closure follows because $\varphi(h)$ is an [automorphism](../../../../automorphism.md) of $N$. To check [associativity](../../../../associative-property.md), calculate both bracketings:

$$
\begin{aligned}
((n,h)(m,k))(r,l)
&=\bigl(n\varphi(h)(m)\varphi(hk)(r),hkl\bigr),\\
(n,h)((m,k)(r,l))
&=\bigl(n\varphi(h)(m\varphi(k)(r)),hkl\bigr)\\
&=\bigl(n\varphi(h)(m)\varphi(h)\varphi(k)(r),hkl\bigr).
\end{aligned}
$$

They agree because $\varphi(hk)=\varphi(h)\varphi(k)$. The identity is $(e_N,e_H)$, using $\varphi(e_H)=\mathrm{id}_N$, and the two-sided inverse is

$$
(n,h)^{-1}=\bigl(\varphi(h^{-1})(n^{-1}),h^{-1}\bigr).
$$

Indeed multiplication in either order gives the identity, using $\varphi(h)\varphi(h^{-1})=\mathrm{id}_N$. This verifies the [group axioms](../../../../group-axioms.md).

For the specified [group presentation](../../../../group-presentation.md), take $N=C_9=\langle X\rangle$ and $H=C_3=\langle Y\rangle$. The rule $\alpha(X)=X^4$ defines an [automorphism](../../../../automorphism.md) because $4$ is coprime to $9$. Furthermore $4^3\equiv1\pmod9$, so $Y\mapsto\alpha$ defines the required [group homomorphism](../../../../group-homomorphism.md) $C_3\to\operatorname{Aut}(C_9)$. In the resulting [semidirect product](../../../../semidirect-product.md) $S$, the canonical generators satisfy

$$
X^9=Y^3=e,\qquad YXY^{-1}=X^4.
$$

Consequently the [group presentation](../../../../group-presentation.md) defines a surjective [group homomorphism](../../../../group-homomorphism.md) $G\to S$, sending $x$ to $X$ and $y$ to $Y$. The underlying [Cartesian product](../../../../cartesian-product.md) gives $|S|=27$, whereas part (a) gives $|G|\le27$. Surjectivity forces equality, so the map is an [isomorphism](../../../../isomorphism.md):

$$
\boxed{G\cong C_9\rtimes_{\alpha}C_3,\qquad\alpha(X)=X^4,\qquad|G|=27.}
$$

This also proves that the $27$ normal forms in part (a) are distinct and that $x$ has [element order](../../../../order-of-a-group-element.md) exactly $9$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
