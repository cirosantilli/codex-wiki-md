<h1 id="12j/solution">Solution</h1>

↑ **Parent:** [12J](../12j.md)

A [linear-feedback shift register](../../../../../linear-feedback-shift-register.md) of length $d$ has binary state $(x_r,\ldots,x_{r+d-1})$ and update

$$
f(v_0,\ldots,v_{d-1})=(v_1,\ldots,v_{d-1},\sum_{j=0}^{d-1}a_jv_j).
$$

Its output obeys $x_{r+d}=\sum_{j=0}^{d-1}a_jx_{r+j}$ over $\mathbb F_2$. Since the state space is finite, its trajectory consists of a transient of length $M$ followed by a cycle of length $N\geq1$, and the output satisfies $x_{r+N}=x_r$ for $r\geq M$.

If the trajectory never reaches zero, all its $M+N$ distinct transient and cyclic states are nonzero; hence $M+N\leq2^d-1$. If it reaches zero, let $M$ be its first zero-state time. The vectors $v,fv,\ldots,f^{M-1}v$ are [linearly independent](../../../../../linear-independence.md): in a dependence, apply $f^{M-1-j}$ where $j$ is the smallest index with a nonzero coefficient; every later term vanishes and the remaining term is $f^{M-1}v\ne0$. Therefore $M\leq d$. The zero cycle has $N=1$, and $d+1\leq2^d-1$ for $d\geq2$. This proves the requested bound for **all $d\geq2$**, and for every invertible register.

The unrestricted printed assertion has one exception: at $d=1$, the zero-feedback register with initial state one outputs $1,0,0,\ldots$. It requires $M\geq1,N\geq1$, so $M+N\geq2>2^1-1$. The universally valid finite-state bound is $M+N\leq2^d$. A register with feedback from its oldest bit is invertible, in which case a nonzero state never reaches zero and the sharper bound holds already with $M=0$.

To recover an unknown register from a known plaintext/ciphertext keystream, the [Berlekamp-Massey algorithm](../../../../../berlekamp-massey-algorithm.md) finds a shortest [linear recurrence](../../../../../linear-recurrence-relation.md) consistent with the observed bits. Use a connection polynomial $C(z)=1+\sum_{j=1}^LC_jz^j$, so the recurrence discrepancy at index $r$ is $\delta=x_r+\sum_{j=1}^LC_jx_{r-j}$. Initialize $C=B=1,L=0,b=1,m=1$. Process the bits in order. If $\delta=0$, increment $m$. If $\delta\ne0$, save $T=C$ and replace

$$
C\longleftarrow C+(\delta/b)z^mB.
$$

If $2L\leq r$, also replace $L$ by $r+1-L$, set $B=T,b=\delta,m=1$; otherwise retain $L,B,b$ and increment $m$. Arithmetic is binary, so every nonzero discrepancy equals one. The stored polynomial $B$ last failed at an earlier index with discrepancy $b$; its shifted contribution cancels the new failure without changing previous successful discrepancies.

Here is the [minimum recurrence length after a new discrepancy](../../../../../minimum-recurrence-length-after-a-new-discrepancy.md) argument behind the update, not just its name. Suppose a span-$L$ recurrence $C$ succeeds through index $r-1$ but fails at $r$. If another polynomial $D$ of span $L'$ succeeded through $r$ and $L+L'\leq r$, compute the [convolution](../../../../../convolution.md) $(CD)x$ at $r$ in two ways. Applying $D$ first gives zero, since all indices $r-j$ used by $C$ lie at least at $L'$. Applying $C$ first gives its nonzero discrepancy at $r$, since its earlier discrepancies used by $D$ vanish and $D_0=1$. This contradiction proves $L'\geq r+1-L$. The shifted-polynomial update attains the larger of the existing minimum length and this new lower bound; induction therefore gives the shortest recurrence for every prefix. Once at least twice the true linear complexity has been observed, this recurrence determines the whole stream: the difference from a true degree-$d$ recurrent stream satisfies a recurrence of degree at most $d+L$, and a prefix of that many zeros forces every later value to be zero. Without any bound on complexity, a finite observed prefix cannot exclude a longer register that diverges later; the breaking claim uses the finite-register hypothesis and adequate known data.

Finally each of the three input streams is eventually periodic. Let $M$ be the maximum of their transient lengths and $N$ a common multiple of their periods. Their joint triple, and hence the bit chosen by the specified rule, repeats after $N$ once $r\geq M$. Therefore

$$
k_{r+M+N}=k_{r+M}\qquad(r\geq0).
$$

This itself is a [linear recurrence](../../../../../linear-recurrence-relation.md) of length $M+N$, so it constructs a [linear-feedback shift register](../../../../../linear-feedback-shift-register.md) producing the selected stream from its first $M+N$ bits. No closure theorem is being assumed: eventual periodicity and this explicit recurrence prove **the combined stream is also an LFSR stream**, even though the combining rule is nonlinear in its three inputs.

## ↑ Ancestors (10)

1. [12J](../12j.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
