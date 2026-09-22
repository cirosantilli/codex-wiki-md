<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Name the upper [graph triangle](../../../../../../triangle-in-a-graph.md)'s vertices $a,b,c$, where $b$ is adjacent to $x$ and $c$ to $y$. Name the middle left vertex $d$ and the lower right vertex $e$. Then $a$ is adjacent to $d$, the lower [graph triangle](../../../../../../triangle-in-a-graph.md) is $d,t,e$, and $e$ is adjacent to $z$.

Suppose $x,y,z$ all have colour $F$, while $t$ has a different colour $T$; denote the third colour by $B$. In the upper [graph triangle](../../../../../../triangle-in-a-graph.md), $b$ and $c$ cannot have colour $F$ and are adjacent, so they have colours $T,B$ in some order and $a$ has colour $F$. In the lower [graph triangle](../../../../../../triangle-in-a-graph.md), $e$ is adjacent to both $t$ and $z$, forcing $e$ to have colour $B$, and then $d$ must have colour $F$. But the edge $ad$ now has equal-coloured endpoints, a contradiction. Thus

$$
\boxed{c(x)=c(y)=c(z)\ne c(t)\text{ cannot occur}.}
$$

For the [three-colour clause gadget](../../../../../../three-colour-clause-gadget.md) used in a reduction, one also needs the converse extension property for Boolean-coloured inputs. With $t=T$ and $x,y,z\in\{T,F\}$, every tuple other than $(F,F,F)$ extends. If $x=T$, take $(a,b,c,d,e)=(T,F,B,F,B)$; this works regardless of $y,z$. If $x=F,y=T$, take $(T,B,F,F,B)$. Finally, if $x=y=F,z=T$, take $(F,T,B,B,F)$. Each assignment satisfies every edge. Therefore this [three-colour clause gadget](../../../../../../three-colour-clause-gadget.md) realizes exactly a three-input disjunction on Boolean inputs.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
