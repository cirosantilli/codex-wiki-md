# Two-lane Markov chain with a deterministic restart

↑ **Parent:** [Markov chain](markov-chain.md)

Take states $0,n,n'$ for $n\geq1$, with $0\to1'$ deterministic and transitions $n\to n-1$ with probability $q$, $n\to(n+1)'$ with probability $p=1-q$, $n'\to n$ with probability $q$, and $n'\to(n+1)'$ with probability $p$. The [Markov chain](markov-chain.md) is transient for $q<q_c$, null recurrent for $q=q_c$, and positive recurrent for $q>q_c$. To see the [Markov chain](markov-chain.md) recurrence threshold, eliminate the primed-state [hitting probabilities](hitting-probability.md) to obtain $p(1+q)a_{n+1}-(1+pq)a_n+qa_{n-1}=0$, with characteristic roots $1$ and $q/(1-q^2)$. Boundedness forces return with probability one when the second root is at least one. When it is below one, the minimal nonnegative solution gives return probability $q^2/p<1$ from $0$. In the positive recurrent case, put $t=(1-q^2)/q$ and $D=q^2+q-1$. The [stationary distribution](stationary-distribution.md) is $\pi_0=D/[q(q+2)]$, $\pi_n=(\pi_0/q)t^{n-1}$ and $\pi_{n'}=\pi_0t^{n-1}$. It follows from balance across each level cut and sums to one; at criticality the invariant weights cannot be normalized.

## ↑ Ancestors (7)

1. [Markov chain](markov-chain.md)
2. [Markov process](markov-process-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/22h/solution.md)
