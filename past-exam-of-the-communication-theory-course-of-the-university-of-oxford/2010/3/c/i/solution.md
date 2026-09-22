<h1 id="3/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let the input probabilities be $(s,t,u)$ and put $v=s+u=1-t$. The output distribution and [conditional entropy](../../../../../conditional-entropy.md) are

$$
q=\left(\frac s2,1-\frac v2,\frac u2\right),\qquad H(Y\mid X)=s+u=v.
$$

For fixed $v$, the first and third output masses [sum](../../../../../sum.md) to $v/2$. Their [entropy](../../../../../information-entropy-split.md) is maximized when they are equal, so $s=u=v/2$. Equivalently, if $v>0$,

$$
H(Y)=h_2(v/2)+(v/2)h_2(s/v)\leq h_2(v/2)+v/2.
$$

The same bound holds at $v=0$ by [continuity](../../../../../continuous-function.md). Therefore $I(X;Y)\leq h_2(v/2)-v/2$, with equality for symmetric outer input probabilities. Writing $z=v/2\in[0,1/2]$, differentiate:

$$
\frac d{dz}(h_2(z)-z)=\log_2\frac{1-z}z-1.
$$

The unique zero is $z=1/3$; strict [concavity](../../../../../concave-function.md) makes it the global maximum. Thus $v=2/3$ and

$$
\boxed{p_X=(1/3,1/3,1/3),\qquad C=h_2(1/3)-1/3=\log_2(3/2).}
$$

The optimum output is $(1/6,2/3,1/6)$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the communication Theory course of the University of Oxford](../../../../split.md)
6. [Communication Theory course of the University of Oxford](../../../../../communication-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
