<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $N=HK=\langle r\rangle$, the [normal subgroup](../../../../../normal-subgroup.md) of order $35$. By [Cauchy's theorem for finite groups](../../../../../cauchy-theorem-for-groups.md), $G$ contains an element $t$ of order two. Such an element cannot belong to the odd-order [subgroup](../../../../../subgroup.md) $N$. Thus $N\cap\langle t\rangle=\{1\}$ and $G=N\langle t\rangle$, giving the [semidirect product](../../../../../semidirect-product.md)

$$
\boxed{G\cong C_{35}\rtimes C_2.}
$$

Every [automorphism of a finite cyclic group](../../../../../automorphism-of-a-finite-cyclic-group.md) sends $r$ to $r^a$ for a [unit](../../../../../unit-in-a-ring.md) $a$ modulo $35$. The relation $t^2=1$ forces the [conjugation action](../../../../../conjugation-action.md) of $t$ to square to the identity:

$$
trt^{-1}=r^a,\qquad a^2\equiv1\pmod{35}.
$$

The [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) identifies a [congruence class](../../../../../congruence-class.md) modulo $35$ with its pair of classes modulo $5$ and $7$. In each of these [prime fields](../../../../../prime-field.md), the factorization $(a-1)(a+1)=0$ forces $a=1$ or $a=-1$. The choices are independent, giving exactly four [homomorphisms from a finite cyclic group](../../../../../homomorphism-from-a-finite-cyclic-group.md) $C_2\to\operatorname{Aut}(C_{35})$. Explicitly,

$$
\boxed{a\equiv1,6,29,34\pmod{35}.}
$$

The factors $C_5$ and $C_7$ of $N$ are preserved by every [automorphism](../../../../../automorphism.md), since each is its unique [subgroup](../../../../../subgroup.md) of that order. The four [conjugation actions](../../../../../conjugation-action.md) therefore give:

- $a=1$: the action is trivial on both factors, so $G\cong C_{35}\times C_2\cong\boxed{C_{70}}$, by [cyclicity of a product of two finite cyclic groups](../../../../../cyclicity-of-a-product-of-two-finite-cyclic-groups.md).
- $a=34$: the action inverts both factors, so $\langle r,t\mid r^{35}=t^2=1,\ trt^{-1}=r^{-1}\rangle$ is the [dihedral group](../../../../../dihedral-group.md) $\boxed{D_{70}}$.
- $a=6$: it is the identity modulo $5$ and inversion modulo $7$, so the $C_5$ factor commutes with the other factors and $G\cong\boxed{D_{14}\times C_5}$.
- $a=29$: it is inversion modulo $5$ and the identity modulo $7$, giving $G\cong\boxed{D_{10}\times C_7}$.

Here $D_n$ has [group order](../../../../../order-of-a-finite-group.md) $n$, as in the paper. The [center of a group](../../../../../center-of-a-group.md) distinguishes these four [groups of order seventy](../../../../../groups-of-order-seventy.md): its orders are $70,1,5,7$, respectively, so the four groups are pairwise nonisomorphic. Each construction is a [semidirect product](../../../../../semidirect-product.md) with $70$ elements, so every listed possibility occurs.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
