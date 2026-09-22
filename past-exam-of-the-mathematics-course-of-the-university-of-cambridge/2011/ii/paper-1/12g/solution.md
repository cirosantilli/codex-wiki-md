<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

Use the square-root encryption convention called the [Rabin-Williams scheme](../../../../../rabin-cryptosystem.md) in [the Cambridge course notes](https://www.dpmms.cam.ac.uk/~twk10/Shan.pdf). Choose distinct large primes $p,q\equiv3\pmod4$, keep them secret, and publish $N=pq$. A message block $m\in\{0,\ldots,N-1\}$ is encrypted as

$$
\boxed{c=m^2\pmod N.}
$$

Usually require $\gcd(m,N)=1$; otherwise the message itself reveals a factor. For a [quadratic residue](../../../../../quadratic-residue.md) $c$ modulo $p$, [Euler criterion](../../../../../euler-criterion.md) gives $c^{(p-1)/2}=1$, so $c^{(p+1)/4}$ is a square root. Compute both signs modulo each prime, then combine the four sign choices by the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md). For a unit ciphertext there are four roots modulo $N$. Message redundancy identifies the intended root; squaring alone does not identify it uniquely.

To reduce [integer factorization](../../../../../integer-factorization.md) to recovery of square roots, choose $x$ uniformly from $(\mathbb Z/N\mathbb Z)^\times$, compute $c=x^2$, and ask the alleged decoder for any root $y$ of $c$. Conditional on $c$, the secret $x$ is uniform among its four roots, even if the decoder deterministically chooses $y$. With probability $1/2$, $y\not\equiv\pm x\pmod N$. Then the signs agree modulo one prime and disagree modulo the other. Since

$$
N\mid(x-y)(x+y),\qquad\boxed{1<\gcd(x-y,N)<N,}
$$

the [greatest common divisor](../../../../../greatest-common-divisor.md) factors $N$. Independent trials require an expected two successful oracle calls. If a trial's chosen $x$ is not a unit, $\gcd(x,N)$ already factors $N$. This establishes the computational equivalence between factorization and inversion of the squaring map; it does not claim that learning any partial information about a formatted message is equivalent to full inversion.

For [coin flipping by telephone](../../../../../coin-flipping-by-telephone.md), Alice publishes $N$ with its factorization secret. Bob chooses uniformly a unit $x$ with $0<x<N/2$ and sends $c=x^2\bmod N$. Alice computes the two roots $r_1,r_2$ in this half interval, selects a binary digit in which they differ, and announces a guess for that digit of Bob's $x$. Bob reveals $x$; Alice verifies its range and square, and their common bit records whether her guess was correct. Alice then reveals $p,q$, so Bob verifies the primes, product, and differing digit.

Conditional on $c$, Bob's original root is equally likely to be $r_1$ or $r_2$, so Alice's guess succeeds with probability $1/2$. Bob cannot change his answer to the other half-interval root without finding a nontrivial second square root, which would factor $N$ by the argument above. Thus, assuming factorization is hard and the prescribed sampling and completed exchange are followed,

$$
\boxed{\mathbb P(\text{Alice wins})=\mathbb P(\text{Bob wins})=\tfrac12.}
$$

The revealed factors make the completed transcript checkable. The protocol does not prevent a party from aborting communication.

## ↑ Ancestors (11)

1. [12G](../12g.md)
2. [Section II](../section-ii.md)
3. [Paper 1](../../paper-1-split.md)
4. [Ii](../../split.md)
5. [2011](../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
