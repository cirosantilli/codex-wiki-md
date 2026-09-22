# Conditional expectation under a martingale density

↑ **Parent:** [Conditional expectation](conditional-expectation.md)

Let $Z_s>0$ be a [martingale](martingale-split.md) with $Z_0=1$ and let $dQ=Z_T\,dP$ on a finite horizon. Its restriction to $\mathcal F_s$ has [Radon-Nikodym derivative](radon-nikodym-derivative.md) $Z_s$. If $Y$ is Q-integrable and $U=\mathbb E_Q[Y\mid\mathcal F_s]$, then for every $A\in\mathcal F_s$,

$$
\mathbb E_P[\mathbf1_AZ_sU]=\mathbb E_Q[\mathbf1_AU]
=\mathbb E_Q[\mathbf1_AY]=\mathbb E_P[\mathbf1_AYZ_T].
$$

Also $Z_sU$ is P-integrable because $\mathbb E_P[Z_s|U|]=\mathbb E_Q|U|<\infty$. The defining uniqueness of [conditional expectation](conditional-expectation.md) gives the displayed formula. In particular, if $N_sZ_s$ is a P-martingale and $N_s$ is Q-integrable, conditioning first at an intermediate time proves $N_s$ is a Q-martingale.

## ↑ Ancestors (7)

1. [Conditional expectation](conditional-expectation.md)
2. [Measure theory](measure-theory-split.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-stochastic-differential-equations-course-of-the-university-of-oxford/2011/3/b/solution.md)
