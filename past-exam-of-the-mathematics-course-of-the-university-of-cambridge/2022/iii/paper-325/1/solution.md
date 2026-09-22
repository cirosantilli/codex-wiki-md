<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $q=(\mathbf q_1,\ldots,\mathbf q_N)$ denote the particle positions. In the [Ghirardi--Rimini--Weber model](../../../../../ghirardi-rimini-weber-theory.md), the wavefunction obeys the ordinary [Schrödinger equation](../../../../../schrodinger-equation.md)

$$
i\hbar\frac{\partial\psi}{\partial t}=H\psi
$$

between random collapses. Each particle $i$ has an independent [Poisson process](../../../../../poisson-process.md) of collapse times with rate $\lambda$. At such a time the state jumps according to

$$
\psi(q)\longmapsto
\frac{L_i(\mathbf X)\psi(q)}{\|L_i(\mathbf X)\psi\|},
\qquad
L_i(\mathbf X)=\frac{1}{(\pi r_C^2)^{3/4}}
\exp\left[-\frac{(\mathbf q_i-\mathbf X)^2}{2r_C^2}\right],
$$

where the random centre has [probability density](../../../../../probability-density.md) $\|L_i(\mathbf X)\psi\|^2$. The normalization is arranged so that $\int d^3X\,L_i(\mathbf X)^2=I$.

The original GRW scales are approximately

$$
r_C\sim10^{-7}\ {\rm m},
\qquad
\lambda\sim10^{-16}\ {\rm s}^{-1}.
$$

An isolated microscopic particle is therefore exceedingly unlikely to collapse during a laboratory experiment. A macroscopic pointer containing about $N\sim10^{23}$ relevant particles has total collapse rate $N\lambda\sim10^7\ {\rm s}^{-1}$ and collapse time about $10^{-7}\ {\rm s}$. After a [measurement interaction](../../../../../measurement-interaction.md) correlates different microscopic outcomes with pointer positions separated by much more than $r_C$, one constituent's localization suppresses all incompatible pointer branches. This [GRW amplification mechanism](../../../../../grw-amplification-mechanism.md) produces one definite macroscopic outcome with probabilities given by the [Born rule](../../../../../born-rule.md), while leaving ordinary microscopic [unitary time evolution](../../../../../unitary-time-evolution.md) almost unchanged.

For one spatial coordinate, average over the random centre of one collapse. The resulting [density operator](../../../../../density-matrix.md) has position-space kernel

$$
\rho'(x,x')=
\exp\left[-\frac{(x-x')^2}{4r_C^2}\right]\rho(x,x').
$$

Its diagonal is unchanged, so $\langle x\rangle$ and $\langle x^2\rangle$ are unchanged. The first derivative of the Gaussian factor vanishes at $x=x'$, so $\langle p\rangle$ is also unchanged. Its second derivative does not vanish, and the [position representation of the momentum operator](../../../../../position-representation-of-the-momentum-operator.md) gives

$$
\boxed{\langle p^2\rangle'
=\langle p^2\rangle+\frac{\hbar^2}{2r_C^2}}.
$$

In three dimensions the increase in total $\mathbf p^2$ is $3\hbar^2/(2r_C^2)$, corresponding to kinetic-energy increase $3\hbar^2/(4mr_C^2)$ per collapse. These are ensemble statements: conditioning on one specified collapse centre can shift the position moments. Repetition at rate $\lambda$ predicts [GRW spontaneous heating](../../../../../grw-spontaneous-heating.md), so precision searches for anomalous bulk heating, spontaneous radiation, momentum diffusion, and loss of matter-wave interference test the model.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 325](../../paper-325-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
