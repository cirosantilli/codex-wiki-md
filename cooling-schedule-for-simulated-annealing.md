# Cooling schedule for simulated annealing

↑ **Parent:** [Simulated annealing](simulated-annealing.md)

A [cooling schedule for simulated annealing](cooling-schedule-for-simulated-annealing.md) specifies successive effective temperatures and how many proposals to attempt at each. For example, $T_k=T_0r^k$ with $0<r<1$, using the [geometric sequence](geometric-progression.md), can define stages of equal chosen length. Changing $T$ changes the [transition matrix](stochastic-matrix.md): if the state [probability distribution](probability-distribution-split.md) is $\mu_n$, then $\mu_{n+1}=\mu_nP_{T_n}$, which generally differs from $\pi_{T_{n+1}}$. Time spent at one temperature must be compared with its [mixing time](mixing-time-of-a-markov-chain.md) before equilibrium intuition is justified.

In the [five-state barrier example for simulated annealing](five-state-barrier-example-for-simulated-annealing.md), fixed $T_*>0$ gives a finite [irreducible Markov chain](irreducible-markov-chain.md), so $4$ is eventually visited with [probability](probability.md) one. That unbounded-time statement gives no fixed finite deadline. Over any finite number $N$ of trials starting at $1$, the [probability](probability.md) of staying at $1$ throughout is

$$
\prod_{n=0}^{N-1}\left[1-\frac12e^{-1/T_n}-\frac12e^{-3/T_n}\right]>0.
$$

Each factor is the rejection [probability](probability.md) at $1$. This is an explicit failure event even when every $T_n$ is positive: the best visited [objective function](objective-function.md) value remains $1$, above the [global minimum](global-minimum.md) value $0$. More exploratory proposals can help cross a barrier; cooling before those moves occur can preserve a poor [local minimum](local-minimum.md). Successful asymptotic schedules need additional analysis of the allowed moves and barriers.

Historically, [Scott Kirkpatrick](scott-kirkpatrick.md), [Charles Daniel Gelatt Jr.](charles-daniel-gelatt-jr.md) and [Mario P. Vecchi](mario-p-vecchi.md) connected [statistical mechanics](statistical-mechanics.md) with [mathematical optimization](mathematical-optimization-split.md) in 1983. They adapted the [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md) to cooling searches with symmetric proposals and illustrated computer-design problems.[Printed pp. 672–673 and 675: Metropolis procedure, cooling schedule, logic partitioning](optimization-by-simulated-annealing-by-scott-kirkpatrick-and-others.md)

## ↑ Ancestors (6)

1. [Simulated annealing](simulated-annealing.md)
2. [Heuristic optimization](heuristic-optimization.md)
3. [Mathematical optimization](mathematical-optimization-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Cooling schedule for simulated annealing](cooling-schedule-for-simulated-annealing.md)
- [Simulated annealing](simulated-annealing.md)
