<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Suppose first that $f=O(g)$. Choose $C>0$ and $N$ so that $|f(n)|\leq C|g(n)|$ for $n\geq N$. There are only finitely many natural numbers below $N$. Because $g(n)\ne0$ at each of them, all ratios $|f(n)|/|g(n)|$ in this finite prefix are finite. Let

$$
c=\max\left(\{C\}\cup\left\{\frac{|f(n)|}{|g(n)|}:n<N\right\}\right).
$$

Then $|f(n)|\leq c|g(n)|$ both in the prefix and in the tail, hence on the entire [domain of a function](../../../../../domain-of-a-function.md). This proves the [finite-prefix extension of a big O bound](../../../../../finite-prefix-extension-of-a-big-o-bound.md).

Conversely, a bound valid for every natural number is certainly valid eventually. The purported real constant cannot be negative because $g$ never vanishes; if it is zero, enlarge it to a positive constant. The definition of [Big O notation](../../../../../big-o-notation.md) then applies. The nonvanishing assumption is what permits the finite exceptions to be absorbed into one constant.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Discrete mathematics, continuous mathematics and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
