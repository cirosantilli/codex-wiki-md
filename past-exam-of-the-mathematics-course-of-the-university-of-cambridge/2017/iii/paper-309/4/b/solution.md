<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $u=t-z$, $\ell=du=e^0-e^3$, $p=A'/A$, $q=B'/B$, with primes denoting $d/du$. The [exterior derivatives](../../../../../../exterior-derivative.md) are $de^0=de^3=0$, $de^1=p\ell\wedge e^1$, $de^2=q\ell\wedge e^2$. For a [Levi-Civita connection](../../../../../../levi-civita-connection.md), the [connection 1-forms](../../../../../../connection-1-form-split.md) obey both [Cartan's first structure equation](../../../../../../cartan-s-first-structure-equation.md) and [metric compatibility](../../../../../../metric-compatibility.md). With lower indices $\omega_{ab}=\eta_{ac}\omega^c{}_b$, the result is

$$
\boxed{\omega_{01}=\omega_{13}=-p\,e^1,\qquad \omega_{02}=\omega_{23}=-q\,e^2,\qquad \alpha=\beta=-\frac{A'}A,\quad \gamma=\delta=-\frac{B'}B.}
$$

All other lower-index forms vanish or follow from $\omega_{ab}=-\omega_{ba}$. Raising the first time index changes its sign: for example $\omega^0{}_1=\omega^1{}_0=p e^1$, whereas $\omega^1{}_3=-p e^1$ and $\omega^3{}_1=p e^1$.

For direct verification, $\omega^1{}_0\wedge e^0+\omega^1{}_3\wedge e^3=-p\ell\wedge e^1=-de^1$, and the same holds for index two. For indices zero and three each term wedges $e^1$ or $e^2$ with itself, so it is zero. These forms are metric-compatible, and uniqueness follows from the [existence and uniqueness of the Levi-Civita connection](../../../../../../existence-and-uniqueness-of-the-levi-civita-connection.md). The printed uniqueness statement implicitly includes metric compatibility: the torsion equation alone permits adding nonzero forms $C^a{}_{bc}e^c$ with $C^a{}_{bc}=C^a{}_{cb}$, since their wedge with $e^b$ vanishes.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 309](../../../paper-309-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
