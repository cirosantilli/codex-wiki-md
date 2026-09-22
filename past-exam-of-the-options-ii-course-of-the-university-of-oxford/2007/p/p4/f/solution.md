<h1 id="p/p4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**The endpoint bounds printed in this part are false.** Take $n=3$, $\epsilon=1/100$ and $\delta=9/10$, which obey $\delta<(n-1)/2-\epsilon=99/100$. The [characteristic polynomial](../../../../../characteristic-polynomial.md) is

$$
P(z)=z^3-6z^2+\frac{2199}{200}z-\frac{4837}{800}.
$$

It has $P(101/100)=-31599/10^6<0$ and $P(5/4)=441/1600>0$, so it has a real root strictly between $1.01$ and $1.25$, outside the first printed interval. There is a unique [eigenvalue](../../../../../eigenvalue.md) in the transpose's isolated first disc of radius $1/4$, identifying it as the first [eigenvalue](../../../../../eigenvalue.md). Similarly $P(301/100)=-40999/10^6<0$ and $P(13/4)=41/64>0$ give a root above $3.01$, violating the last printed interval. The approximate three roots are $1.02675615$, $1.94385374$ and $3.02939011$.

There is nevertheless a corrected enclosure proving the claimed reality. Under the stated condition write $R=\epsilon+\delta<(n-1)/2$. The large first row disc is disjoint from the large last column disc, since their centres are $n-1$ apart and their radii are both $R$. Every [eigenvalue](../../../../../eigenvalue.md) lies both in the row union and in the column union. It cannot belong to both large discs, so it lies in at least one of the fixed small discs

$$
S_1:\ |z-1|\le1/4,\qquad S_i:\ |z-i|\le1/4+\epsilon\ (2\le i\le n-1),\qquad S_n:\ |z-n|\le1/4.
$$

These fixed discs are pairwise disjoint. At $\delta=0$ each contains one [eigenvalue](../../../../../eigenvalue.md). Eigenvalues depend continuously, as a multiset, on the entries; throughout the [connected](../../../../../connected-space.md) allowed interval no [eigenvalue](../../../../../eigenvalue.md) can move between these separated fixed sets while remaining in their union. Thus each still contains one, counted with multiplicity. Complex-conjugate pairing now proves each is real. The valid conclusion is

$$
\boxed{|\lambda_1-1|\le1/4,\quad|\lambda_i-i|\le1/4+\epsilon\ (2\le i\le n-1),\quad|\lambda_n-n|\le1/4}.
$$

The source's stronger width $\epsilon$ at both endpoints does not persist after adding the corner entry; it was valid for the unperturbed matrix only.

The enclosure method is [Complementary row and column Gershgorin isolation](../../../../../complementary-row-and-column-gershgorin-isolation.md).

## ↑ Ancestors (13)

1. [F](../f.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
