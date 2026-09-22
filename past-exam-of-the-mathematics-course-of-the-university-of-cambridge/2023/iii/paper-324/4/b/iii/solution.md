<h1 id="4/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

If $S|\alpha\rangle=|\alpha\rangle$ and $|\beta\rangle=U|\alpha\rangle$, then

$$
(USU^\dagger)|\beta\rangle
=US|\alpha\rangle
=U|\alpha\rangle
=|\beta\rangle.
$$

Thus conjugating the state conjugates its entire [stabilizer group](../../../../../../../stabilizer-group.md).

The triangle $G_B$ is obtained from the path $G_A$ by [local complementation of a graph state](../../../../../../../local-complementation-of-a-graph-state.md) at vertex $2$, which toggles the edge between its neighbors $1$ and $3$. The corresponding [Local Clifford operation](../../../../../../../local-clifford-operation.md) is

$$
U_2=exp\left(-\frac{i\pi}{4}X_2\right)
\exp\left(\frac{i\pi}{4}Z_1\right)
\exp\left(\frac{i\pi}{4}Z_3\right).
$$

Direct conjugation gives

$$
U_2S_1^AU_2^\dagger=Y_1Y_2=S_1^BS_2^B,
$$



$$
U_2S_2^AU_2^\dagger=S_2^B,
$$



$$
U_2S_3^AU_2^\dagger=Y_2Y_3=S_2^BS_3^B.
$$

These three commuting operators generate exactly the same [stabilizer group](../../../../../../../stabilizer-group.md) as $S_1^B,S_2^B,S_3^B$. Therefore

$$
\boxed{|G_B\rangle=e^{i\phi}U_2|G_A\rangle}
$$

for an irrelevant global phase $e^{i\phi}$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 324](../../../../paper-324-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
