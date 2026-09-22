<h1 id="8d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [modular Heisenberg group](../../../../../../modular-heisenberg-group.md), the three independent entries each have $p$ choices, so

$$
\boxed{|H_p|=p^3.}
$$

The multiplication and commutation calculations work over the [finite field](../../../../../../finite-field.md) $\mathbb F_p$ exactly as over $\mathbb R$. Taking $x'=1,z'=0$ and $x'=0,z'=1$ shows that

$$
Z(H_p)=\{M(0,y,0):y\in\mathbb F_p\}.
$$

Let $c=M(0,1,0)$. Its powers exhaust the centre and $c$ has order $p$, giving the [group presentation](../../../../../../group-presentation.md)

$$
\boxed{Z(H_p)=\langle c\mid c^p=e\rangle\cong C_p.}
$$

Let $a=M(1,0,0)$ and $b=M(0,0,1)$. Their images $\bar a,\bar b$ in the [quotient group](../../../../../../quotient-group.md) translate the $x,z$ entries independently. They commute modulo the centre, have order $p$, and generate $p^2$ distinct pairs. Therefore

$$
\boxed{H_p/Z(H_p)=\langle\bar a,\bar b\mid\bar a^p=\bar b^p=e,\ \bar a\bar b=\bar b\bar a\rangle\cong C_p\times C_p.}
$$

For context, $aba^{-1}b^{-1}=c$, with $c$ central. All conclusions above include $p=2$; one must not infer that every nonidentity element of $H_2$ has order two, since $(ab)^2=c$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [8D](../../8d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
