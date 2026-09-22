<h1 id="33d/solution">Solution</h1>

↑ **Parent:** [33D](../33d.md)

The [angular momentum commutation relations](../../../../../angular-momentum-commutation-relations.md) imply

$$
[S_z,S_\pm]=\pm\hbar S_\pm,
\qquad [\mathbf S^2,S_\pm]=0.
$$

Thus $S_\pm|s,\sigma\rangle$ has the same total-spin [eigenvalue](../../../../../eigenvalue.md) and magnetic quantum number $\sigma\pm1$. Its squared norm follows from

$$
S_\mp S_\pm=\mathbf S^2-S_z^2\mp\hbar S_z:
$$



$$
\lVert S_\pm|s,\sigma\rangle\rVert^2
=\hbar^2\left[s(s+1)-\sigma(\sigma\pm1)\right].
$$

Choosing the conventional positive phases gives the [spin ladder operator](../../../../../spin-ladder-operator.md) formula

$$
\boxed{S_\pm|s,\sigma\rangle
=\hbar\sqrt{s(s+1)-\sigma(\sigma\pm1)}
|s,\sigma\pm1\rangle}.
$$

For $s=1$, in the ordered basis $|1,1\rangle,|1,0\rangle,|1,-1\rangle$,

$$
S_+=\sqrt2\hbar
\begin{pmatrix}0&1&0\\0&0&1\\0&0&0\end{pmatrix},
\qquad S_-=S_+^\dagger.
$$

Since $S_x=(S_++S_-)/2$,

$$
\boxed{S_x=\frac{\hbar}{\sqrt2}
\begin{pmatrix}0&1&0\\1&0&1\\0&1&0\end{pmatrix}}.
$$

The incident state is the [spin coherent state](../../../../../spin-coherent-state.md) obtained by rotating $|1,1\rangle$ through $\theta$ about the $y$ axis. Its amplitudes in the $S_z$ basis are

$$
\langle1,1|\mathbf n,+\rangle=\cos^2\frac\theta2,
\qquad
\langle1,0|\mathbf n,+\rangle=\frac{\sin\theta}{\sqrt2},
\qquad
\langle1,-1|\mathbf n,+\rangle=\sin^2\frac\theta2,
$$

up to an irrelevant phase convention. The [Born rule](../../../../../born-rule.md) therefore gives

$$
\boxed{\frac{N_+}{N_-}
=\frac{\cos^4(\theta/2)}{\sin^4(\theta/2)}
=\cot^4\frac\theta2}.
$$

## ↑ Ancestors (10)

1. [33D](../33d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
