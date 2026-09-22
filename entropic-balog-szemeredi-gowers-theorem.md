<h1 id="entropic-balog-szemeredi-gowers-theorem">Entropic Balog-Szemerédi-Gowers theorem</h1>

↑ **Parent:** [Entropic Ruzsa distance](entropic-ruzsa-distance.md)

For finitely supported random variables $A,B$ in an [abelian group](abelian-group.md),

$$
d_R(A;B\mathbin\Vert A+B)
\leq 3I(A;B)+2H(A+B)-H(A)-H(B).
$$

To prove it, take two conditionally independent copies $(A_1,B_1)$ and $(A_2,B_2)$ of $(A,B)$ given $A+B$. Since $A_1+B_1=A_2+B_2$, [entropy submodularity](entropy-submodularity.md) gives

$$
H(A_1-B_2)
\leq H(A_1-B_2,A_1)+H(A_1-B_2,B_1)-H(A_1-B_2,A_1,B_1).
$$

The first two terms are at most $H(A)+H(B)$. The last joint entropy is

$$
2H(A,B)-H(A+B).
$$

Consequently $H(A_1-B_2)\leq H(A+B)+2I(A;B)$. Subtracting

$$
H(A\mid A+B)=H(B\mid A+B)
=H(A)+H(B)-I(A;B)-H(A+B)
$$

from this bound proves the theorem.

## ↑ Ancestors (6)

1. [Entropic Ruzsa distance](entropic-ruzsa-distance.md)
2. [Information theory](information-theory-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-164/4/i/solution.md)
