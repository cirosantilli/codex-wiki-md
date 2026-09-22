<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $q=|B|$ and choose $h$ uniformly from the finite family $H$. All bounds below must hold for every pair of distinct inputs $x,y\in A$.

A [universal hash family](../../../../../universal-hash-family.md), also called universal2, satisfies $P[h(x)=h(y)]\leq1/q$. A [strongly universal hash family](../../../../../strongly-universal-hash-family.md) satisfies

$$
P[h(x)=u,\ h(y)=v]=q^{-2}\quad\text{for every }u,v\in B.
$$

Thus the two outputs are independent and uniform; summing over $u=v$ gives the collision condition. An [almost strongly universal hash family](../../../../../almost-strongly-universal-hash-family.md) permits a larger conditional guessing bound. In the $\varepsilon$-almost-strongly-universal convention used here,

$$
P[h(x)=u]=q^{-1},\qquad P[h(x)=u,\ h(y)=v]\leq\varepsilon/q,
$$

equivalently $P[h(y)=v\mid h(x)=u]\leq\varepsilon$. Necessarily $\varepsilon\geq1/q$, with $\varepsilon=1/q$ giving strong universality. Stating this normalization matters because the name alone does not specify the allowed forgery [probability](../../../../../probability.md).

Here is an explicit [polynomial almost strongly universal hashing](../../../../../polynomial-almost-strongly-universal-hashing.md) construction and a one-use [message authentication](../../../../../message-authentication.md) protocol. Use a publicly specified [finite field](../../../../../finite-field.md) $\mathbb F_q$, where $q=2^t$. Encode a fixed-length $n$-bit message as $L=\lceil n/t\rceil$ field elements $m_1,\ldots,m_L$, padding the final block in a fixed way. Both parties know the length, so this encoding is injective. They share independent uniform secret field elements $a,b$, requiring $2t$ shared secret bits. Define

$$
h_{a,b}(m)=b+\sum_{j=1}^{L}m_ja^j.
$$

For every message, the output is uniform because of $b$. For distinct messages $m,m'$ and prescribed tags $u,v$, the condition $h(m)=u$ determines exactly one value of $b$ for each $a$. The remaining condition is

$$
\sum_{j=1}^{L}(m'_j-m_j)a^j=v-u.
$$

Its left-hand side has a nonzero coefficient of positive degree, so subtracting the specified constant gives a nonzero [polynomial](../../../../../polynomial-split.md) of degree at most $L$. By the [root bound for a polynomial](../../../../../lagrange-root-bound-over-a-field.md), there are at most $L$ possible field elements $a$. Consequently

$$
P[h(m)=u,h(m')=v]\leq L/q^2,
$$

and this is an $\varepsilon$-almost-strongly-universal family with $\varepsilon=L/q$, provided $L<q$. The powers start at one deliberately: a message coefficient at power zero could give a known constant tag shift, allowing a deterministic substitution.

Alice sends the message and its tag $u=h_{a,b}(m)$ over the public channel. Bob accepts only if his independently computed tag agrees. An attacker who has seen no tag guesses one with [probability](../../../../../probability.md) $1/q$. After seeing a valid pair $(m,u)$, an attacker substituting a different message $m'$ and any chosen tag $v$ succeeds with conditional [probability](../../../../../probability.md) at most $L/q$. This remains true when the choice of $m',v$ depends on the observed pair: the bound is uniform over all those choices. More explicitly, the observed tag leaves $a$ uniform because each possible $a$ has exactly one compatible secret mask $b$.

For a desired forgery bound $\eta$, choose $t=\lceil\log_2(n/\eta)\rceil$. Since $L\leq n$ and $q\geq n/\eta$, the substitution bound is at most $\eta$. The secret requirement is

$$
\boxed{2t=O(\log n+\log(1/\eta))\text{ bits},\qquad P(\text{substitution accepted})\leq L/2^t\leq\eta.}
$$

For a long message this is much shorter than its $n$ bits. This is [Wegman–Carter authentication](../../../../../wegman-carter-authentication.md): a keyed hash plus a fresh secret [one-time pad](../../../../../one-time-pad.md) on the tag. It authenticates the message rather than concealing its contents. Use the key once for the guarantee just established; multiple authenticated messages require fresh masks and a reuse security analysis. Authenticate lengths and sequence identifiers too if variable lengths or replay protection are required.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 54](../../paper-54-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
