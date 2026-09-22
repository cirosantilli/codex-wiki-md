<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Take $a_1,a_2>0$ and $p_1+p_2=1$. Write $g^{(k)}=\nabla u$ in phase $k$ and $h^{(k)}=a_kg^{(k)}$. Here $h$ is the positive conductivity flux; physical [heat flux](../../../../../../heat-flux-density.md) is $-h$. Continuity of [temperature](../../../../../../temperature.md) on a planar interface implies continuity of its tangential derivatives, while conservation gives continuity of normal [heat flux](../../../../../../heat-flux-density.md). With interface normal $e_1$, these conditions are

$$
g^{(1)}_2=g^{(2)}_2=E_2,\qquad
g^{(1)}_3=g^{(2)}_3=E_3,\qquad
a_1g^{(1)}_1=a_2g^{(2)}_1=h_1.
$$

The mean [gradient](../../../../../../gradient.md) is $E=p_1g^{(1)}+p_2g^{(2)}$. Therefore

$$
E_1=h_1\left(\frac{p_1}{a_1}+\frac{p_2}{a_2}\right),\qquad
\langle h_2\rangle=(p_1a_1+p_2a_2)E_2,\qquad
\langle h_3\rangle=(p_1a_1+p_2a_2)E_3.
$$

By the definition of [effective conductivity](../../../../../../effective-conductivity.md), $\langle h\rangle=a^*E$. Thus

$$
\boxed{
a^*=\operatorname{diag}\left(
\frac{a_1a_2}{p_1a_2+p_2a_1},\
p_1a_1+p_2a_2,\
p_1a_1+p_2a_2
\right).
}
$$

The [laminate conductivity](../../../../../../laminate-conductivity.md) is a weighted [harmonic mean](../../../../../../harmonic-mean.md) across the layers and a weighted [arithmetic mean](../../../../../../arithmetic-mean.md) along them. This also explains why [isotropic](../../../../../../isotropy.md) constituents can yield an [anisotropic](../../../../../../anisotropy.md) [thermal conductivity tensor](../../../../../../thermal-conductivity-tensor.md): flux must cross each resistance in sequence in the normal direction, whereas tangential transport occurs in parallel.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
