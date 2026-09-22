<h1 id="22h/solution">Solution</h1>

↑ **Parent:** [22H](../22h.md)

Read the arrows in the original diagram as follows: $0$ moves to $1'$ with probability one; from an unprimed $n\geq1$, probability $q$ leads to $n-1$ and probability $p$ leads to $(n+1)'$; from $n'$ the corresponding destinations are $n$ and $(n+1)'$. This is the [two-lane Markov chain with a deterministic restart](../../../../../two-lane-markov-chain-with-a-deterministic-restart.md). It is irreducible: every state can reach zero by a finite path of $q$ transitions, and zero can reach every primed state by outward $p$ transitions and then every unprimed state by a $q$ transition. Thus all states have the same recurrence classification.

Let $a_n$ and $b_n$ be the [hitting probabilities](../../../../../hitting-probability.md) of zero starting from $n$ and $n'$, with $a_0=1$. First-step conditioning gives

$$
a_n=qa_{n-1}+pb_{n+1},\qquad b_n=qa_n+pb_{n+1}\quad(n\geq1).
$$

Subtracting yields $b_n=(1+q)a_n-qa_{n-1}$. Eliminating $b_{n+1}$ gives

$$
p(1+q)a_{n+1}-(1+pq)a_n+qa_{n-1}=0.
$$

Its characteristic roots are $1$ and $r=q/[p(1+q)]=q/(1-q^2)$. Put $q_c=(\sqrt5-1)/2$, so $r=1$ precisely when $q=q_c$.

For $q>q_c$, the general solution is $a_n=A+Br^n$. The bound $0\leq a_n\leq1$ and $r>1$ force $B=0$, and $a_0=1$ then gives $a_n=b_n=1$. For $q=q_c$, the general solution is $a_n=A+Bn$; boundedness again gives $a_n=b_n=1$. In both cases, the return probability from zero is $b_1=1$, so the [Markov chain](../../../../../markov-chain.md) is recurrent.

For $q<q_c$, $0<r<1$, and the pair

$$
a_n=r^n,\qquad b_n=q(1+q)r^n
$$

is a nonnegative bounded solution of the first-step equations. To identify it as the actual [hitting probability](../../../../../hitting-probability.md), use that [hitting probability is the minimal nonnegative harmonic extension](../../../../../hitting-probability-is-the-minimal-nonnegative-harmonic-extension.md). This fact follows directly by iteration: a nonnegative solution with boundary value one at zero dominates the probability of hitting zero within $N$ steps, for every $N$. The actual bounded solution has form $a_n=A+(1-A)r^n$, where nonnegativity as $n\to\infty$ requires $A\geq0$. Minimality bounds it above by $r^n$, while this form bounds it below by $r^n$. Hence it is exactly the displayed solution. Starting at zero, the [first return time](../../../../../first-return-time.md) has finite-return probability $b_1=q^2/p<1$. The [Markov chain](../../../../../markov-chain.md) is therefore transient.

It remains to distinguish positive and null recurrence. Write $u_n=\pi_n$ and $v_n=\pi_{n'}$ for invariant probabilities. Balance at zero and at $1'$ gives $\pi_0=qu_1$ and $v_1=\pi_0$. For the finite cut consisting of zero and both lanes up to level $n$, invariance equates its outward and inward probability fluxes:

$$
p(u_n+v_n)=qu_{n+1}.
$$

Balance at the unprimed state $n$ also gives $u_n=q(u_{n+1}+v_n)$. Combining these identities yields

$$
v_n=qu_n,\qquad u_{n+1}=t u_n,\qquad t=\frac{p(1+q)}q=\frac{1-q^2}q.
$$

Therefore every invariant probability distribution would necessarily have $u_n=(\pi_0/q)t^{n-1}$ and $v_n=\pi_0t^{n-1}$. Conversely, these weights satisfy all individual balance equations, including $v_{n+1}=p(u_n+v_n)$, so their summability is the only remaining condition.

When $q>q_c$, $t<1$, and normalization gives

$$
\boxed{\pi_0=\frac{q^2+q-1}{q(q+2)},\qquad
\pi_n=\frac{\pi_0}{q}\left(\frac{1-q^2}{q}\right)^{n-1},\qquad
\pi_{n'}=\pi_0\left(\frac{1-q^2}{q}\right)^{n-1}\quad(n\geq1).}
$$

An [irreducible Markov chain](../../../../../irreducible-markov-chain.md) has an invariant probability distribution exactly when it is [positive recurrent](../../../../../positive-recurrent-markov-chain.md); equivalently its mean return time is finite and $\pi_0$ is its reciprocal. Thus this case is positive recurrent. At $q=q_c$, $t=1$ and the nonzero invariant weights cannot be summed to one. Irreducibility would force $\pi_0>0$ in any invariant probability distribution. Since recurrence was already proved but no such distribution exists, this case is [null recurrent](../../../../../null-recurrent-state.md).

The complete classification is therefore **transient for $0<q<q_c$, null recurrent at $q=q_c$, and positive recurrent for $q_c<q<1$**. A drift argument using only the unprimed arrows would miss the primed lane and give the wrong threshold.

## ↑ Ancestors (10)

1. [22H](../22h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
