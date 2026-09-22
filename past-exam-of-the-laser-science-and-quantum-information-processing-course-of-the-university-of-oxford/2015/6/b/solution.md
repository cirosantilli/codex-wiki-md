<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In the [oracle machine](../../../../oracle-machine.md) model, a function is accessed through a black box whose internal gate cost is excluded; the resource counted is the number of calls. A reversible classical oracle maps basis inputs as $(x,y)\mapsto(x,y\oplus f(x))$. Its [quantum oracle](../../../../quantum-oracle.md) extension applies the same permutation coherently to arbitrary superpositions, without measuring its input. A classical random mixture of inputs is not that coherent extension.

Write the two truth-table entries as $f(0)=b$, $f(1)=a\oplus b$. Then $f(x)=ax\oplus b$, with the four cases

$$
\begin{array}{c|c|c|c}
(a,b)&f(0)&f(1)&f(x)\\\hline
(0,0)&0&0&0\\
(0,1)&1&1&1\\
(1,0)&0&1&x\\
(1,1)&1&0&1\oplus x
\end{array}.
$$

Two classical query circuits, $(0,0)\xrightarrow{U_f}(0,f(0))$ and $(1,0)\xrightarrow{U_f}(1,f(1))$, recover the whole function with certainty. One call fixes only one entry, leaving two compatible functions; hence two are necessary classically. Randomization cannot remove this obstruction to certainty.

The minimum for **full exact function identification remains two even with coherent quantum queries**. To see this, expand the oracle target into its $X$ eigenstates: it is identity on $|+\rangle$, and gives phases $(-1)^{f(x)}$ on $|x\rangle|-\rangle$. Any one-query input, including an auxiliary system, has orthogonal sector weights $w_+$, $w_0$ and $w_1$ summing to one. The output overlap between functions differing only at $0$ is $1-2w_0$, so perfect distinction requires $w_0=1/2$; differing only at $1$ likewise requires $w_1=1/2$. Then $w_+=0$, but functions differing at both entries have overlap $1-2(w_0+w_1)=-1$. They are the same ray rather than distinguishable states. Thus one query cannot identify all four functions. The following one-query task recovers only whether the entries agree.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
