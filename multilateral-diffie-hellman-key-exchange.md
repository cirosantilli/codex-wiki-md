# Multilateral Diffie-Hellman key exchange

↑ **Parent:** [Diffie-Hellman key exchange](diffie-hellman-key-exchange.md)

In a [cyclic group](cyclic-group.md) with generator $g$, $n$ participants with secret exponents $a_j$ can exchange $n$ tokens around a ring. Token $j$ starts at $g^{a_j}$ and is successively exponentiated by its next $n-2$ recipients before being sent to the final recipient, whose exponent is the only one missing. That recipient completes the exponentiation locally. Each token makes $n-1$ transmissions, and everyone obtains $g^{\prod_j a_j}$. Thus $n(n-1)$ transmitted group elements suffice. As with two-party [Diffie-Hellman key exchange](diffie-hellman-key-exchange.md), authentication is needed.

## ↑ Ancestors (6)

1. [Diffie-Hellman key exchange](diffie-hellman-key-exchange.md)
2. [Coding theory](coding-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ii/paper-4/4h/solution.md)
