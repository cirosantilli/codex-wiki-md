<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Use one transition per time step in the printed [discrete-time multi-state diagnosis model](../../../../../../discrete-time-multi-state-diagnosis-model.md). Put $a=\delta_E$, $b=\delta_N$, and $r=1-b$. Let $I_k=S_{1k}\sim\operatorname{Poisson}(h_k(\theta))$ be the new infection count. Let $U_k$ be the undiagnosed non-early count present in state 3 at step $k$, including those retained by its self-loop. Start with $I_0=U_0=0$.

For the realised [random variables](../../../../../../random-variable-split.md), define conditionally

$$
E_k\mid I_{k-1}\sim\operatorname{Binomial}(I_{k-1},a),\qquad
D_k\mid U_{k-1}\sim\operatorname{Binomial}(U_{k-1},b),
$$

using independent individual transition choices, and set

$$
\boxed{S_{2k}=E_k,\quad
U_k=I_{k-1}-E_k+U_{k-1}-D_k,\quad
S_{4k}=D_k.}
$$

The early split's two complementary counts are not independent conditional on $I_{k-1}$, nor are the late split's two counts conditional on $U_{k-1}$. **Random state incidences must not be equated to their expectations.**

Explicitly, the first four realised vectors are

$$
\begin{aligned}
S_1&=(I_1,0,0,0),\\
S_2&=(I_2,E_2,I_1-E_2,0),\\
S_3&=(I_3,E_3,I_2-E_3+I_1-E_2-D_3,D_3),\\
S_4&=(I_4,E_4,I_3-E_4+I_2-E_3+I_1-E_2-D_3-D_4,D_4).
\end{aligned}
$$

Here $E_k$ and $D_k$ have the conditional laws just given; $D_1=D_2=0$. The corresponding expressions solely in terms of the parameters are the mean flow vectors. Writing $h_j=h_j(\theta)$ and interpreting state 3 with its self-loop as $S_{3k}=U_k$, they are

$$
\begin{aligned}
\mathbb E S_1&=(h_1,0,0,0),\\
\mathbb E S_2&=(h_2,ah_1,(1-a)h_1,0),\\
\mathbb E S_3&=(h_3,ah_2,(1-a)(h_2+rh_1),b(1-a)h_1),\\
\mathbb E S_4&=(h_4,ah_3,(1-a)(h_3+rh_2+r^2h_1),b(1-a)(h_2+rh_1)).
\end{aligned}
$$

These follow from $\mathbb E U_k=(1-a)h_{k-1}+r\mathbb E U_{k-1}$. They make the minimum one-step early delay and two-step late delay explicit. If “entering state 3” is reserved for first entry only, its incidence is $I_{k-1}-E_k$ with mean $(1-a)h_{k-1}$; $U_k$ is then a separate occupancy variable. The late-diagnosis expressions are unchanged. This distinction resolves the wording's use of incidence alongside a state-3 self-loop.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
