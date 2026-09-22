<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [height](../../../../../height-of-an-ideal.md) of a prime ideal $P$ is

$$
\operatorname{ht}P=\sup\{n:P_0\subsetneq P_1\subsetneq\cdots\subsetneq P_n=P
\text{ are prime}\}.
$$

The [Krull principal ideal theorem](../../../../../krull-principal-ideal-theorem.md) states that if $R$ is Noetherian and $P$ is minimal among the primes containing a proper principal ideal $(a)$, then

$$
\boxed{\operatorname{ht}P\leq1.}
$$

Suppose otherwise that $P_0\subsetneq Q\subsetneq P$. Quotient by $P_0$ and localize at $P$; it is enough to consider a Noetherian local domain whose maximal ideal $P$ is the only prime containing $(a)$ and which has $0\subsetneq Q\subsetneq P$.

For $n\geq1$, put

$$
Q^{(n)}=Q^nR_Q\cap R.
$$

This is a $Q$-primary ideal. Since $R/(a)$ is a zero-dimensional [Noetherian ring](../../../../../noetherian-ring.md), it is [Artinian](../../../../../artinian-ring.md), and the descending chain $(Q^{(n)}+(a))/(a)$ eventually stabilizes. Thus, for all sufficiently large $n$, every $q_n\in Q^{(n)}$ can be written

$$
q_n=q_{n+1}+ra,\qquad q_{n+1}\in Q^{(n+1)}.
$$

Now $ra\in Q^{(n)}$, while $a\notin Q$; $Q$-primaryness gives $r\in Q^{(n)}$. Hence

$$
Q^{(n)}=Q^{(n+1)}+aQ^{(n)}.
$$

The [Nakayama lemma](../../../../../nakayama-lemma.md) applied to $Q^{(n)}/Q^{(n+1)}$ gives $Q^{(n)}=Q^{(n+1)}$. Localizing at $Q$ makes all sufficiently large powers of the nonzero maximal ideal $QR_Q$ equal. A nonzero element of the stable power then belongs to $\bigcap_nQ^nR_Q$, contradicting the [Krull intersection theorem](../../../../../krull-intersection-theorem.md). This proves the theorem.

Now let $R$ be a Noetherian [integral domain](../../../../../integral-domain.md). If $R$ is a [unique factorization domain](../../../../../unique-factorization-domain.md) and $P$ has height one, choose $0\ne x\in P$ and an irreducible factor $p$ of $x$. In a UFD, $p$ is prime, so

$$
(0)\subsetneq(p)\subseteq P.
$$

Height one forces $P=(p)$.

Conversely, suppose every height-one prime is principal. Noetherianity makes $R$ an [atomic domain](../../../../../atomic-domain.md). Given an [irreducible element](../../../../../irreducible-element.md) $p$, choose a prime $P$ minimal over $(p)$. The principal ideal theorem gives $\operatorname{ht}P=1$, so $P=(q)$ by hypothesis. Since $p=qr$ and $p$ is irreducible, $r$ is a unit; hence $(p)=P$ is prime. Thus every irreducible is a [prime element](../../../../../prime-element.md), and an atomic domain with this property is a UFD. Therefore

$$
\boxed{R\text{ is a UFD}\quad\Longleftrightarrow\quad
\text{every height-one prime of }R\text{ is principal}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 148](../../paper-148-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
