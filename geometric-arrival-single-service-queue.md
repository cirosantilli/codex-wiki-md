# Geometric-arrival single-service queue

↑ **Parent:** [Queueing theory](queueing-theory-split.md)

Let the independent arrivals satisfy $\Pr(G_n=j)=qp^j$, with $p+q=1$. During a [busy period](busy-period.md), each served customer produces $G_n$ further customers, so the total number served has the total-progeny law of a [Galton-Watson process](galton-watson-process.md) with mean $p/q$. Its extinction probability solves $s=q/(1-ps)$ and is the smaller of $1$ and $q/p$. The queue is positive recurrent for $p<1/2$, null recurrent for $p=1/2$, and transient for $p>1/2$. In the positive recurrent case its [stationary distribution](stationary-distribution.md) is $\pi_j=(1-p/q)(p/q)^j$.

## ↑ Ancestors (6)

1. [Queueing theory](queueing-theory-split.md)
2. [Probability theory](probability-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-2/20c/solution.md)
