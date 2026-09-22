<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $F=K(\mathbb Z/4,1)$, $E=K(\mathbb Z,2)$, and $B=K(\mathbb Z,2)$. In total degree at most two, the $E_2$ page of the mod-two [Serre spectral sequence](../../../../../../serre-spectral-sequence.md) has

$$
E_2^{0,0}=E_2^{0,1}=E_2^{0,2}=E_2^{2,0}=\mathbb F_2,
$$

and $E_2^{1,0}=E_2^{1,1}=0$. A periodic free resolution of the cyclic group gives $H_1(F;\mathbb Z)=\mathbb Z/4$ and $H_2(F;\mathbb Z)=0$. Hence $H^1(F;\mathbb F_2)\cong\operatorname{Hom}(\mathbb Z/4,\mathbb F_2)$, while the [universal coefficient theorem for cohomology](../../../../../../universal-coefficient-theorem-for-cohomology.md) gives $H^2(F;\mathbb F_2)\cong\operatorname{Ext}(\mathbb Z/4,\mathbb F_2)$; both are one-dimensional.

The edge map $H^2(B;\mathbb F_2)\to H^2(E;\mathbb F_2)$ is induced by multiplication by $4$ and is therefore zero modulo two. Consequently

$$
d_2:E_2^{0,1}\longrightarrow E_2^{2,0}
$$

is an isomorphism. The differential out of $E_2^{0,2}$ is zero, because the total space has a one-dimensional $H^2$ which must survive in filtration zero. Thus for every $r\geq3$ and $p+q\leq2$,

$$
E_r^{0,0}=E_r^{0,2}=\mathbb F_2
$$

and all other groups in that range vanish.

It follows that

$$
H^0(F;\mathbb F_2)=H^1(F;\mathbb F_2)=H^2(F;\mathbb F_2)=\mathbb F_2.
$$

The surviving filtration-zero class is the restriction of the degree-two class of $E$, so

$$
\boxed{\operatorname{im}H^2(f;\mathbb F_2)=H^2(F;\mathbb F_2).}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 165](../../../paper-165-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
