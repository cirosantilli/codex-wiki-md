# First-return decomposition of a Dyck path

↑ **Parent:** [Dyck path](dyck-path.md)

A nonempty [Dyck path](dyck-path.md) starts with $U$. At its first later return to height zero, cut after the matching $D$. The segment between these two steps stays at height at least one; translating it down one level gives a [Dyck path](dyck-path.md) $P$. The remaining suffix is another [Dyck path](dyck-path.md) $Q$. This gives the unique form $UPDQ$.

If the original [semilength of a Dyck path](semilength-of-a-dyck-path.md) is $n$ and that of $P$ is $k$, then $Q$ has [semilength of a Dyck path](semilength-of-a-dyck-path.md) $n-1-k$. The first return occurs after $2(k+1)$ steps. For the illustrated path `UUUDDDUD`, $n=4$, $P$ is `UUDD`, $Q$ is `UD`, and the first return occurs after six steps.

<a id="image-first-return-decomposes-a-dyck-path-and-explains-the-catalan-recurrence"></a>
![](catalan-first-return-decomposition.png)

**[Figure 16](#image-first-return-decomposes-a-dyck-path-and-explains-the-catalan-recurrence). First return decomposes a Dyck path and explains the Catalan recurrence**. Original chosen path of semilength four. Purple steps enclose a blue two-pair path; the orange suffix has one pair. The bar chart independently counts all paths of semilength four by the inside semilength $k$: the four groups have sizes $5,2,2,5$, totaling $14$. The highlighted group contains the displayed path.

## ↑ Ancestors (6)

1. [Dyck path](dyck-path.md)
2. [Lattice path](lattice-path.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Catalan number](catalan-number.md)
- [Catalan recurrence](catalan-recurrence.md)
