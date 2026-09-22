<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define $H(X\mid Y)=\sum_y\mathbb P(Y=y)H(X\mid Y=y)$. The joint [entropy](../../../../information-entropy-split.md) identity $H(X,Y)=H(Y)+H(X\mid Y)$ follows by writing $p_{xy}=q_yp_{x\mid y}$ and expanding its logarithm. If $Y=g(X)$, then $H(Y\mid X)=0$ and $H(X,Y)=H(X)$, giving the desired decomposition.

[Group](../../../../group-split.md) the first two symbols together and keep the third separate. If $c<1$, the identity becomes

$$
H(a,b,c)=h(c)+(1-c)h\!\left(\frac a{1-c}\right),
$$

where $h(t)=-t\log_2t-(1-t)\log_2(1-t)$. [Binary entropy](../../../../binary-entropy.md) is at most one, with equality precisely at $1/2$. Hence

$$
H(a,b,c)\le h(c)+1-c=H((1-c)/2,(1-c)/2,c).
$$

Equality holds exactly when $a=b=(1-c)/2$. When $c=1$, $a=b=0$, so the same conclusion holds at the boundary.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
