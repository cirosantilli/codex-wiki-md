# Floquet growth rate

↑ **Parent:** [Floquet theory](floquet-theory.md)

The [Floquet growth rate](floquet-growth-rate.md) measures the exponential trend of a periodic [linear differential equation](linear-differential-equation.md) over many coefficient periods. A [Floquet multiplier](floquet-multiplier.md) $m$ measures the factor per period $T$; the corresponding rate per unit time is

$$
\gamma_m=\frac{\log|m|}{T}=\operatorname{Re}\rho_m,\qquad e^{T\rho_m}=m,
$$

where $\rho_m$ is a [Floquet exponent](floquet-exponent.md). Taking the [real part](real-part.md) removes the ambiguity in the complex [logarithm](logarithm.md).

For the scalar example under [periodic solution](periodic-solution.md), $m=e^{2\pi a}$ and the [Floquet growth rate](floquet-growth-rate.md) is $a$, independently of $b$. Indeed,

$$
\frac{1}{t}\log\frac{y(t)}{y(0)}=a+b\frac{\sin t}{t}\longrightarrow a,\qquad \frac{y'(t)}{y(t)}=a+b\cos t.
$$

The instantaneous [logarithmic derivative](logarithmic-derivative.md) keeps oscillating even though its average over complete periods is exactly $a$. Sampling at the same phase in each period removes the modulation altogether: $y(nT)=m^ny(0)$.

<a id="image-the-multiplier-gives-a-factor-per-period-and-its-logarithm-gives-a-rate-per-unit-time"></a>
![](floquet-stroboscopic-multiplier-and-rate.png)

**[Figure 15](#image-the-multiplier-gives-a-factor-per-period-and-its-logarithm-gives-a-rate-per-unit-time). The multiplier gives a factor per period and its logarithm gives a rate per unit time**. Left: sampling $y'=\left(a+\cos t\right)y$ at $t=nT$, $T=2\pi$, gives $y(nT)=m^n$; straight lines on the logarithmic scale have slopes $\log m$ per period. Right: the instantaneous logarithmic derivatives $a+\cos t$ oscillate around the constant long-term rates $a=-0.2,0,+0.2$.

For the general finite-dimensional homogeneous [linear differential equation](linear-differential-equation.md) $x'=A(t)x$, assume that $A$ is continuous on the real line and $T$-periodic, with $T>0$. Normalize its [fundamental matrix](fundamental-matrix-of-a-linear-differential-equation.md) by $\Phi(0)=I$ and set $M=\Phi(T)$. The maximal asymptotic exponential rate, using any induced [matrix norm](matrix-norm.md), is

$$
\gamma=\lim_{t\to\infty}\frac{\log\|\Phi(t)\|}{t}=\frac{\log\rho(M)}{T},\qquad \rho(M)=\max_j|m_j|.
$$

Here $\rho(M)$ is the [spectral radius](spectral-radius.md), $m_j$ are the [Floquet multipliers](floquet-multiplier.md), and invertibility gives $\rho(M)>0$. This concerns growth of the solution operator; it does not say that every [initial condition](initial-condition.md) attains the maximum.[§3.6, printed pp. 91–93, equation (3.120), Theorem 3.15 and the multiplier/exponent relation](ordinary-differential-equations-and-dynamical-systems-by-gerald-teschl.md)

To prove the formula, write $t=nT+s$ with $0\leq s<T$. Periodicity and uniqueness give

$$
\Phi(t)=\Phi(s)M^n.
$$

Both $\Phi(s)$ and $\Phi(s)^{-1}$ have uniformly bounded [matrix norms](matrix-norm.md) on a period. Consequently $\|\Phi(t)\|$ differs from $\|M^n\|$ by at most fixed multiplicative factors. The [spectral radius formula](spectral-radius-formula.md) gives $\|M^n\|^{1/n}\to\rho(M)$, proving the claimed limit without choosing a [matrix logarithm](matrix-logarithm.md).

For a particular nonzero [initial condition](initial-condition.md) $v$, decompose $v$ into the [generalized eigenspaces](generalized-eigenspace.md) of $M$ over the complex numbers. The rate of $\Phi(t)v$ is the largest $T^{-1}\log|m_j|$ among components that are nonzero. Generic data have a component in the dominant [generalized eigenspaces](generalized-eigenspace.md) and attain $\gamma$; data contained in the sum of the subdominant [generalized eigenspaces](generalized-eigenspace.md) have a smaller rate. For example, with $A=\operatorname{diag}(0.2,-0.3)$, the maximal rate is $0.2$, while $v=(0,1)$ decays at rate $-0.3$. These [invariant subspaces](invariant-subspace.md) describe initial data at phase zero. Their transported versions $E(t)=\Phi(t)E(0)$ can vary with time and satisfy $E(t+T)=E(t)$.

A negative [Floquet growth rate](floquet-growth-rate.md) allows temporary amplification. For the constant [non-normal matrix](non-normal-matrix.md)

$$
A=\begin{pmatrix}-1&10\\0&-1\end{pmatrix},\qquad e^{tA}=e^{-t}\begin{pmatrix}1&10t\\0&1\end{pmatrix},
$$

the [initial condition](initial-condition.md) $v=(0,1)$ has Euclidean [norm](norm.md) $e^{-t}\sqrt{100t^2+1}$, which rises from $1$ to about $3.697$ at $t=1$ before eventually decaying. Its exponential rate is still $-1$: the [Jordan block](jordan-block.md) contributes a polynomial factor, whose [logarithm](logarithm.md) divided by $t$ tends to zero. At a unit-modulus [Floquet multiplier](floquet-multiplier.md), such polynomial growth can even be unbounded with zero exponential rate; $A=\left(\begin{smallmatrix}0&1\\0&0\end{smallmatrix}\right)$ gives $e^{tA}v=(t,1)$. Thus zero [Floquet growth rate](floquet-growth-rate.md) alone proves neither boundedness nor a [periodic solution](periodic-solution.md).

## ↑ Ancestors (8)

1. [Floquet theory](floquet-theory.md)
2. [Linear differential equation](linear-differential-equation.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (6)

- [Floquet growth rate](floquet-growth-rate.md)
- [Floquet multiplier](floquet-multiplier.md)
- [Monodromy matrix of a periodic linear system](monodromy-matrix-of-a-periodic-linear-system.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-318/2/solution.md)
- [Periodic solution](periodic-solution.md)
- [Periodically reversing Parker dynamo coupling](periodically-reversing-parker-dynamo-coupling.md)
