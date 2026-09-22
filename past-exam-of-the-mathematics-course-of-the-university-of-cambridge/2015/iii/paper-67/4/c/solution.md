<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each interaction neighbourhood, set

$$
G_s^{(Z)}=\int_{\mathbb R}w(t)
e^{itH_s}h_Ze^{-itH_s}\,dt.
$$

Then the shell term is $g^{(Z,s)}=G_s^{(Z)}-G_{s-1}^{(Z)}$. Since $H_0=h_Z$, its conjugation leaves $h_Z$ fixed, so $G_0^{(Z)}=h_Z\int w=h_Z$. Since $H_D=H$, $G_D^{(Z)}$ is precisely the choice of $g^{(Z)}$ from (b). Therefore the [telescoping local-shell decomposition](../../../../../../telescoping-local-shell-decomposition.md) gives

$$
\boxed{h_Z+\sum_{s=1}^Dg^{(Z,s)}
=G_0^{(Z)}+\sum_{s=1}^D
(G_s^{(Z)}-G_{s-1}^{(Z)})
=G_D^{(Z)}=g^{(Z)}.}
$$

No limiting interchange is needed: the sum has finitely many shells. Each $G_s^{(Z)}$ is supported within the union of supports appearing in $H_s$ together with $Z$, because its [unitary time evolution](../../../../../../unitary-time-evolution.md) acts trivially outside that neighbourhood. The individual shell terms need not commute with the full [ground state](../../../../../../ground-state.md) projector; the full filtered sum does.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
