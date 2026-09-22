<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Start with $R_0=A$. Having chosen disjoint $A_1,\ldots,A_i$, put $R_i=A\setminus\bigcup_{j\leq i}A_j$ and

$$
s_i=\sup\{\mu(B):B\in\mathfrak M,\ B\subseteq R_i\}.
$$

The empty set shows $s_i\geq0$, and finite total variation bounds it above. If $s_i>0$, choose $A_{i+1}\subseteq R_i$ with $\mu(A_{i+1})\geq s_i/2>0$; if $s_i=0$, choose $A_{i+1}=\varnothing$. This is the required recursion, including the initial step $i=0$.

Disjointness and nonnegativity give $\sum_i\mu(A_i)\leq|\mu|(A)<\infty$, hence $\mu(A_i)\to0$. Write $R=A\setminus\bigcup_i A_i$. For every measurable $B\subseteq R$,

$$
\mu(B)\leq s_i\leq2\mu(A_{i+1})\longrightarrow0.
$$

Thus every measurable subset of $R$ has nonpositive [measure](../../../../../measure-split.md). Each finite partition of $R$ consequently has variation sum exactly $-\mu(R)$, and therefore $|\mu|(R)=-\mu(R)$. It follows that $\mu^+(R)=0$. Finally [countable additivity](../../../../../countable-additivity.md) gives

$$
\boxed{\mu(R)=\mu(A)-\sum_i\mu(A_i)\leq\mu(A)<0,\qquad\mu^+(R)=0.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../../split.md)
6. [Real and harmonic analysis course of the University of Oxford](../../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
