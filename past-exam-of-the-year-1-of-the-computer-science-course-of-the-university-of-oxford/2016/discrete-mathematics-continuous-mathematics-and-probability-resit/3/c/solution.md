<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Interpret $\mathbb R_+$ as the strictly positive reals, as in the domain $x>0$ in question 1(e). A bound valid for every $n$ is immediately an eventual bound, by taking $m=0$ (or the least natural number under the other convention).

Conversely, suppose the eventual [big O notation](../../../../../big-o-notation.md) bound holds with constants $m,c$. Since $g(j)>0$, all the finitely many ratios $|f(j)|/|g(j)|$ with $j<m$ are finite. Choose

$$
C=\max\left(1,c,\left\{\frac{|f(j)|}{|g(j)|}:j<m\right\}\right),
$$

omitting the set of ratios when it is empty. For $n<m$ the definition of $C$ gives $|f(n)|\leq C|g(n)|$, and for $n\geq m$ the original bound does so. Hence **the two definitions are equivalent for the stated strictly positive codomain**.

Strict positivity matters. If $\mathbb R_+$ were instead intended to include zero, an eventual bound need not extend to all indices: $g(0)=0$, $f(0)=1$, and $f(n)=g(n)=1$ for $n\geq1$ give a counterexample. More generally, extension is possible exactly when each initial zero of $g$ is also a zero of $f$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Discrete mathematics, continuous mathematics and probability (resit)](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
