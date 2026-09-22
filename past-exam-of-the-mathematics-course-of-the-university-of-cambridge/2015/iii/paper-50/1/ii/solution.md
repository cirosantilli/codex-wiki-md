<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write the [rapidity](../../../../../../rapidity.md) parameters as $\kappa_i=\cosh\theta_i$, $\beta_i=\sinh\theta_i$, and define $E_i=e^{X_i}$. The signed coefficient in the [Sine-Gordon multisoliton tau representation](../../../../../../sine-gordon-multisoliton-tau-representation.md) is

$$
a_{12}=e^{B_{12}}=\frac{1-\cosh(\theta_1-\theta_2)}{1+\cosh(\theta_1-\theta_2)}=-\alpha_{12},\qquad \alpha_{12}=\tanh^2\frac{\theta_1-\theta_2}{2}.
$$

For distinct [rapidities](../../../../../../rapidity.md), $0<\alpha_{12}<1$. In particular, $B_{12}$ cannot be taken as a real logarithm of a positive coefficient. The finite sums defining the [Hirota tau functions](../../../../../../hirota-tau-function.md) can instead be evaluated directly with the real, negative $a_{12}$. They give

$$
f=1-\alpha_{12}E_1E_2,\qquad g=E_1+E_2.
$$

The physical field is a continuous [branch of a multivalued function](../../../../../../branch-of-a-multivalued-function.md), equivalently $\phi=4\arg(f+ig)$ with the argument followed continuously. The principal [inverse tangent](../../../../../../inverse-tangent.md) alone jumps when $f$ changes sign.

Follow the first [kink](../../../../../../scalar-field-kink.md) with $x=v_1t+O(1)$. Then $X_1=O(1)$ and $X_2=\kappa_2(v_1-v_2)t+O(1)$. The two possible local limits are

$$
\begin{aligned}
E_2\longrightarrow0 &: \quad \phi\longrightarrow4\arctan E_1,\\
E_2\longrightarrow\infty &: \quad \frac gf\longrightarrow-\frac1{\alpha_{12}E_1},\quad \phi\longrightarrow2\pi+4\arctan(\alpha_{12}E_1),
\end{aligned}
$$

where the second field is written on the continuous [kink](../../../../../../scalar-field-kink.md) branch. Thus both limits are single [Sine-Gordon kinks](../../../../../../sine-gordon-kink.md) of the same width and velocity, but their centers obey $X_1=0$ or $X_1+\log\alpha_{12}=0$. Following the second [kink](../../../../../../scalar-field-kink.md) gives the same conclusion with labels exchanged. The incoming and outgoing velocities are therefore

$$
\boxed{v_i=\frac{\beta_i}{\kappa_i}=\tanh\theta_i\quad(i=1,2).}
$$

There is no change in the asymptotic [rapidities](../../../../../../rapidity.md) or [kink](../../../../../../scalar-field-kink.md) profiles.

Define the spatial shift as the outgoing center intercept minus the incoming center intercept. Since the large-$E_2$ limit occurs afterwards when $v_1>v_2$, and beforehand when $v_1<v_2$, the [soliton time delay](../../../../../../soliton-time-delay.md) is

$$
\boxed{\Delta x_{1|2}=-\frac{\operatorname{sgn}(v_1-v_2)}{\kappa_1}\log\alpha_{12},\qquad \Delta^{(2)}t[v_1;v_2]=\frac{\operatorname{sgn}(v_1-v_2)}{\beta_1}\log\alpha_{12}.}
$$

The time formula uses $\Delta t=-\Delta x/v_1$ and requires $v_1\ne0$. Its dependence on the velocities is explicit on substituting

$$
\alpha_{12}=\frac{1-v_1v_2-\sqrt{(1-v_1^2)(1-v_2^2)}}{1-v_1v_2+\sqrt{(1-v_1^2)(1-v_2^2)}},\qquad \frac1{\beta_1}=\frac{\sqrt{1-v_1^2}}{v_1}.
$$

For a faster right-moving [kink](../../../../../../scalar-field-kink.md), $\Delta x_{1|2}>0$ and $\Delta t<0$: it arrives earlier than its freely continued incoming trajectory. If $v_1=0$, report the finite spatial shift; a fixed-position arrival-time delay for a stationary [kink](../../../../../../scalar-field-kink.md) is undefined. Coincident velocities are excluded from a separated collision asymptotic.

For completeness, allowing [antikinks](../../../../../../antikink.md) means $\kappa_i=\sigma_i\cosh\theta_i$, $\beta_i=\sigma_i\sinh\theta_i$, with $\sigma_i=\pm1$. The velocities remain $\tanh\theta_i$. For opposite orientations, $|a_{12}|=\coth^2[(\theta_1-\theta_2)/2]$, and the general spatial shift is

$$
\Delta x_{1|2}=-\frac{\operatorname{sgn}[\kappa_2(v_1-v_2)]}{\kappa_1}\log|a_{12}|.
$$

This follows from the same two local limits; it makes explicit the orientation hypothesis behind the velocity-only all-[kink](../../../../../../scalar-field-kink.md) answer.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
