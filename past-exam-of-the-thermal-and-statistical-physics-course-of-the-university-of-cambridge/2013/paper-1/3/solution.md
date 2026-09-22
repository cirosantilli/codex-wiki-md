<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $z=e^{\beta(\mu-\epsilon)}$. For one nondegenerate fermionic [quantum state](../../../../quantum-state.md), the allowed occupations 0 and 1 give $\Xi_F=1+z$. For a bosonic state, summing all nonnegative occupations gives $\Xi_B=(1-z)^{-1}$, requiring $z<1$ or $\mu<\epsilon$. Differentiating the logarithm,

$$
\bar n=z\frac{\partial\ln\Xi}{\partial z},\qquad
\boxed{\bar n_F=\frac1{e^{\beta(\epsilon-\mu)}+1},\qquad
\bar n_B=\frac1{e^{\beta(\epsilon-\mu)}-1}.}
$$

The [interacting point defect](../../../../single-orbital-interacting-defect.md) has two distinct [spin](../../../../spin.md) states, not one fermionic state. Its four [microstates](../../../../microstate.md) have grand-canonical weights $1,z,z,qz^2$, with $q=e^{-\beta U}$. The first two single-electron weights are separate up/down [spin](../../../../spin.md) possibilities; the double state has one [electron](../../../../electron.md) of each [spin](../../../../spin.md). Thus

$$
\Xi=1+2z+qz^2,\qquad
\boxed{\bar n=\frac{2z+2qz^2}{1+2z+qz^2}.}
$$

For $U=0$, $\Xi=(1+z)^2$ and $\bar n=2z/(1+z)$. The sketch is a single smooth step from 0 to 2, centred on $\mu=\epsilon$, where $\bar n=1$. As $T\to0$ its width tends to zero.

For positive U with $\beta U\gg1$, the lowest grand energies are successively $0$, $\epsilon-\mu$ and $2\epsilon+U-2\mu$. Away from the two crossings,

$$
\boxed{\bar n\simeq\begin{cases}
0,&\mu<\epsilon,\\
1,&\epsilon<\mu<\epsilon+U,\\
2,&\mu>\epsilon+U.
\end{cases}}
$$

Finite [temperature](../../../../temperature-split.md) smooths each step over an [energy](../../../../energy-split.md) range of order $k_BT$. Near the lower step double occupation is exponentially suppressed, so $\bar n\simeq2z/(1+2z)$. Near the upper step put $y=e^{\beta(\mu-\epsilon-U)}$ and neglect the empty state, giving $\bar n\simeq1+y/(2+y)$. [Spin degeneracy](../../../../spin-degeneracy.md) shifts the half-step positions to $\epsilon-k_BT\ln2$ and $\epsilon+U+k_BT\ln2$.

For a grand-canonical probability $p_s\propto e^{-\beta(E_s-\mu n_s)}$, differentiation gives $\partial_\mu p_s=\beta(n_s-\bar n)p_s$. Multiplying by $n_s$ and summing proves

$$
\boxed{\sigma^2=k_BT\left(\frac{\partial\bar n}{\partial\mu}\right)_T.}
$$

For this defect, direct state counting gives

$$
\langle n^2\rangle=\frac{2z+4qz^2}{\Xi},\qquad
\sigma^2=\frac{2z(1+2qz+qz^2)}{(1+2z+qz^2)^2}.
$$

At $\mu=\epsilon$, $z=1$ and therefore

$$
\boxed{\sigma^2=\frac{2+6e^{-\beta U}}{(3+e^{-\beta U})^2}\longrightarrow\frac29.}
$$

The same limit gives $\bar n=2/3$: empty, up and down states have equal weights, while the double state is suppressed. Replacing this degeneracy by a two-outcome equal-weight model would incorrectly give [variance](../../../../variance-split.md) $1/4$ at this [chemical potential](../../../../chemical-potential-split.md).

Across the full chemical-potential range the [variance](../../../../variance-split.md) has two well-separated narrow peaks and tends to zero on the 0, 1 and 2 plateaux. The limiting shapes are $2z/(1+2z)^2$ near the lower step and $2y/(2+y)^2$ near the upper one. Each peak has height $1/4$, at the shifted half-step position; the [variance](../../../../variance-split.md) at the unshifted crossings is instead $2/9$.

<a id="3/image-original-grand-canonical-defect-occupations-and-number-variance-showing-the-interaction-induced-one-electron-plateau-and-spin-degeneracy-shifts-of-the-variance-peaks"></a>
![](../../../../past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2013/paper-1-tsp2013-defect-statistics.png)

**[Figure 5](#3/image-original-grand-canonical-defect-occupations-and-number-variance-showing-the-interaction-induced-one-electron-plateau-and-spin-degeneracy-shifts-of-the-variance-peaks). Original grand-canonical defect occupations and number variance, showing the interaction-induced one-electron plateau and spin-degeneracy shifts of the variance peaks**.

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2013](../../split.md)
4. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../split.md)
5. [Thermal and Statistical Physics course of the University of Cambridge](../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
