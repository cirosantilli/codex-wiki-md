<h1 id="b/4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Retain the whole price history when calculating the arithmetic average. The [Asian option](../../../../../asian-option.md) payoffs at expiry are

$$
\boxed{\begin{array}{c|c|c|c}
\text{path}&(S_0,S_1,S_2)&A_2&(115-A_2)^+\\\hline
uu&(100,120,144)&364/3&0\\
ud&(100,120,120)&340/3&5/3\\
du&(100,100,120)&320/3&25/3\\
dd&(100,100,100)&100&15
\end{array}}
$$

In particular $ud$ and $du$ have the same terminal stock price but different averages and payoffs. The average is an additional state variable; the terminal stock nodes cannot be merged for this claim.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
