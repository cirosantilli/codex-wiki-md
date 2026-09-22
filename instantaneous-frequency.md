# Instantaneous frequency

↑ **Parent:** [Frequency modulation](frequency-modulation.md)

For a [signal](signal.md) with a specified differentiable, continuously unwrapped [wave phase](phase-waves.md) $\phi(t)$, its instantaneous frequency is

$$
f_i(t)=\frac{1}{2\pi}\frac{d\phi}{dt}.
$$

Unwrapping means following successive turns instead of resetting the [wave phase](phase-waves.md) at $2\pi$. Differentiating a reset phase would introduce artificial jumps. An arbitrary real [signal](signal.md) does not by itself specify a unique amplitude-phase representation; this definition refers to the phase chosen in the model.

For the single-message-[frequency](frequency.md) [FM](frequency-modulation.md) model,

$$
\phi(t)=2\pi f_ct+\beta\sin(2\pi f_mt),\qquad
f_i(t)=f_c+\beta f_m\cos(2\pi f_mt).
$$

The proof is the [chain rule](chain-rule.md): the [derivative](derivative.md) of the [sine](sine.md) contributes $2\pi f_m$, which cancels the $2\pi$ in the definition. In the $20\,\mathrm{Hz}$ example, $f_i(0)=25$, $f_i(1/4)=20$, and $f_i(1/2)=15\,\mathrm{Hz}$. Although the [frequency](frequency.md) offset vanishes at $t=1/4$, the [wave phase](phase-waves.md) offset is then $5$ [radians](radian.md); the [wave phase](phase-waves.md) offset and its rate of change need not vanish together.

Between times $t_1,t_2$, the accumulated number of cycles is $(\phi(t_2)-\phi(t_1))/(2\pi)=\int_{t_1}^{t_2}f_i(t)\,dt$. Thus a crossing-to-crossing measurement yields an average [frequency](frequency.md) over that interval. Its reciprocal time is only an approximation to the [instantaneous frequency](instantaneous-frequency.md) at one point when $f_i$ varies slowly over a cycle.

## ↑ Ancestors (3)

1. [Frequency modulation](frequency-modulation.md)
2. [Electrical engineering](electrical-engineering-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Frequency deviation](frequency-deviation.md)
- [Frequency modulation](frequency-modulation.md)
- [Instantaneous frequency](instantaneous-frequency.md)
- [Single-tone FM sidebands](single-tone-fm-sidebands.md)
