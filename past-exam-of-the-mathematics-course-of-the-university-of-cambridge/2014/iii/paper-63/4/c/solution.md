<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a fixed original term, define $F_d(h_Z)=\int w(t)e^{itH_d}h_Ze^{-itH_d}dt$. The shell increment is exactly $A^{(Z,d)}=F_d(h_Z)-F_{d-1}(h_Z)$. Hence the [telescoping local-shell decomposition](../../../../../../telescoping-local-shell-decomposition.md) gives

$$
\sum_{d=1}^DA^{(Z,d)}=F_D(h_Z)-F_0(h_Z).
$$

Use the printed endpoint convention $H_0=h_Z$ and $H_D=H$. The first endpoint is $F_0(h_Z)=h_Z\int w=h_Z$, because $h_Z$ commutes with its own evolution, and the second is the operator chosen in part (b). Thus

$$
\boxed{A^{(Z)}=h_Z+\sum_{d=1}^DA^{(Z,d)}.}
$$

There is a distance-convention issue in the endpoint assertion. The usual minimum distance between supports is zero for overlapping distinct interactions, so a literal $H_0=\sum_{Y:d(Z,Y)=0}h_Y$ need not equal $h_Z$ or commute with it. To realize the stated $H_0=h_Z$, index the neighborhoods by distance between interaction terms: the central term has shell zero, and other terms begin in positive shells. For example, for distinct terms use one plus their support [interaction distance](../../../../../../interaction-distance.md). With the ordinary overlapping-support convention left unchanged, the exact formula instead begins with $F_0(h_Z)$, not necessarily with $h_Z$. The telescoping identity itself is valid in either convention.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
