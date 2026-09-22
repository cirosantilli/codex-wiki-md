# Delayed cursor feedback experiment

↑ **Parent:** [Feedback delay](feedback-delay.md)

Can [feedback delay](feedback-delay.md) change correction timing even when the physical task stays the same? Susilaradeya and colleagues tested this in a human tracking experiment. Participants pressed with both index fingers against fixed [force](force.md) sensors; the two forces controlled a screen cursor along two diagonal axes. A target moved in slow [circular motion](circular-motion.md), usually at $0.2$ rotations per second. The researchers sampled the forces at $50$ samples per second and inserted an additional delay of $0$, $100$, $200$, $300$, or $400$ milliseconds before displaying the cursor. Each trial lasted $20$ seconds; the $70$ trials included $14$ per delay, in pseudorandom order. [Susilaradeya et al., Extrinsic and intrinsic dynamics in movement intermittency (2019), figure 1 and human task methods](https://pmc.ncbi.nlm.nih.gov/articles/PMC6453565/)

The readout was fluctuation in cursor [angular velocity](angular-velocity.md), analyzed by [Fourier transforms](fourier-transform.md) over approximately $10$ seconds from the middle of each trial. The principal peak was around $2$ hertz without added delay, around $1.4$ hertz with $100$ milliseconds, and around $1$ hertz with $200$ milliseconds. Thus changing observation timing changed the timing of corrective motion. [Susilaradeya et al., results: submovement frequencies are affected by feedback delays](https://pmc.ncbi.nlm.nih.gov/articles/PMC6453565/) This is an empirical motivation for taking stale observations seriously. Human [feedback control](closed-loop-control.md) includes prediction and other dynamics; these observations do not measure $k$ in the ideal integrator model or test its $k\tau=\pi/2$ boundary.

## ↑ Ancestors (6)

1. [Feedback delay](feedback-delay.md)
2. [Closed-loop control](closed-loop-control.md)
3. [Control theory](control-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
