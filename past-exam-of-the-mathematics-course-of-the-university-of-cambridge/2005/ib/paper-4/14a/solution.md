<h1 id="14a/solution">Solution</h1>

↑ **Parent:** [14A](../14a.md)

For nonempty $F$, the [triangle inequality](../../../../../triangle-inequality.md) gives $d(x,z)\leq d(x,y)+d(y,z)$ for every $z\in F$. Taking the infimum yields $d(x,F)\leq d(x,y)+d(y,F)$. Interchanging $x,y$ proves

$$
\boxed{|d(x,F)-d(y,F)|\leq d(x,y).}
$$

Thus the [distance to a set](../../../../../distance-to-a-set.md) is a [Lipschitz function](../../../../../lipschitz-continuity.md), hence continuous. If $x\notin F$ and $F$ is closed, its open complement contains a ball $B(x,\epsilon)$; every point of $F$ is at least $\epsilon$ away. Hence $\boxed{d(x,F)>0}$ for $x\notin F$.

For two nonempty disjoint closed sets, let $h(x)=d(x,F_1)-d(x,F_2)$. It is continuous, negative on $F_1$ and positive on $F_2$. The disjoint open sets $U_1=\{h<0\}$ and $U_2=\{h>0\}$ contain them. Empty sets cause no difficulty, using an empty neighborhood for the empty set. This proves **every metric space is a [normal topological space](../../../../../normal-space.md)**.

In any normal space, a closed $F$ contained in an open $U$ can be separated from $X\setminus U$: choose disjoint open $W\supset F$ and $V\supset X\setminus U$. Because $X\setminus V$ is closed and contains $W$, $\overline W\subset X\setminus V\subset U$. First choose disjoint open $U_1,U_2$ around $F_1,F_2$, then apply this argument separately to each pair $F_i\subset U_i$. It gives $\overline W_i\subset U_i$, and therefore $\boxed{\overline W_1\cap\overline W_2=\varnothing}$. This is [closed-neighborhood shrinking in a normal space](../../../../../closed-neighborhood-shrinking-in-a-normal-space.md).

For the two specified hyperbola branches, explicit choices are

$$
\boxed{W_1=\{(x,y):x<0,\ xy<-1/2\},\qquad W_2=\{(x,y):x>0,\ xy>1/2\}.}
$$

They are open and contain the branches with products $-1$ and $1$. Their closures lie respectively in $\{x\leq0,xy\leq-1/2\}$ and $\{x\geq0,xy\geq1/2\}$. Any common point would have $x=0$, making both product inequalities impossible. Thus their closures are disjoint even though the original branches can approach one another arbitrarily closely at large height.

## ↑ Ancestors (10)

1. [14A](../14a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
