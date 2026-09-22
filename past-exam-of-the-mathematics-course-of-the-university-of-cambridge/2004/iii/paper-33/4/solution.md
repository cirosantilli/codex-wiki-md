<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a [transferable utility game](../../../../../transferable-utility-game.md), the [characteristic function of a coalitional game](../../../../../characteristic-function-of-a-coalitional-game.md) assigns a [coalition](../../../../../coalition-game-theory.md) $S$ its largest total attainable revenue $v(S)$, with $v(\varnothing)=0$. The [core of a cooperative game](../../../../../core-game-theory.md) consists of payoff vectors $x$ satisfying efficiency, $x(N)=v(N)$, and [coalition](../../../../../coalition-game-theory.md) stability, $x(S)\geq v(S)$ for every $S$. A [coalition](../../../../../coalition-game-theory.md) receiving less could operate alone and distribute its extra value to make each member better off.

Use thousands of pounds as the monetary unit. The physical directed arcs are $A\to B$ and $C\to D$, owned by $i$, with capacities $3,2$; $A\to C$ and $B\to D$, owned by $j$, with capacities $1,1$; and $B\to C$, owned by $k$, with capacity $2$.

<a id="4/image-company-ownership-and-capacities-in-the-two-demand-communication-network"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33-owned-network.png)

**[Figure 1](#4/image-company-ownership-and-capacities-in-the-two-demand-communication-network). Company ownership and capacities in the two-demand communication network**.

The physical network is acyclic. There are exactly three $A$–$D$ [graph paths](../../../../../path-in-a-graph.md) and one $B$–$C$ [graph path](../../../../../path-in-a-graph.md). Let $u,v,w$ be the $A$–$D$ flows on $ABD$, $ACD$, $ABCD$, respectively, and let $z$ be the direct $B$–$C$ demand. Their capacities and revenue are

$$
u+w\leq3,\quad u\leq1,\quad v\leq1,\quad
v+w\leq2,\quad w+z\leq2,\quad u,v,w,z\geq0,
\qquad R=6(u+v+w)+4z.
$$

Every feasible traffic pattern decomposes into these [graph paths](../../../../../path-in-a-graph.md), so these inequalities are exact. The first is redundant, since $u\leq1$ and $w\leq2$ imply it.

Formulate this as a [minimum-cost flow](../../../../../minimum-cost-flow-problem.md) through the [two-resource path packing as minimum-cost circulation](../../../../../two-resource-path-packing-as-minimum-cost-circulation.md) reduction. Use auxiliary [vertices](../../../../../vertex-graph-theory.md) $s,L,R,t$ and the following arcs, whose entries are (capacity, cost):

$$
\begin{array}{c|c}
s\to t&(1,-6)\\
s\to L&(2,0)\\
L\to t&(1,-6)\\
L\to R&(\infty,-6)\\
s\to R&(\infty,-4)\\
R\to t&(2,0)\\
t\to s&(\infty,0)
\end{array}
$$

The first forward [graph path](../../../../../path-in-a-graph.md) carries $u$, $sLt$ carries $v$, $sLRt$ carries $w$, and $sRt$ carries $z$. Conservation at $L$ imposes $v+w\leq2$, and at $R$ imposes $w+z\leq2$; the individual finite-capacity arcs give the other bounds. The return arc closes the circulation. Its cost is exactly $-R$, so this is an ordinary minimum-cost circulation with precisely the required feasible traffic set. Unlimited capacities may all be replaced by $5$, the [maximum](../../../../../maximum-of-a-subset-of-a-total-order.md) possible total [graph path](../../../../../path-in-a-graph.md) flow.

An [linear programming optimality certificate](../../../../../linear-programming-optimality-certificate.md) is particularly short:

$$
R=6u+4v+2(v+w)+4(w+z)
\leq6+4+4+8=22.
$$

The feasible choice $u=v=w=z=1$ attains equality. Thus the actual traffic is three units from $A$ to $D$ and one from $B$ to $C$, and

$$
\boxed{R_{\max}=\text{£}22000.}
$$

All four positive terms in the bound must be tight at any optimum, so these [graph path](../../../../../path-in-a-graph.md) amounts are unique.

The two traffic demands must retain their identities. Merely adding fictitious return arcs $D\to A$ and $C\to B$ to the physical [graph](../../../../../graph-split.md) can create an invalid [graph cycle](../../../../../cycle-in-a-graph.md) combining both rewards: $A\to C\to B\to D\to A$ would credit the $j$-only network with revenue even though it carries neither requested demand. The resource-flow formulation above avoids that problem.

For the [characteristic function](../../../../../characteristic-function.md), only complete physical [graph paths](../../../../../path-in-a-graph.md) owned by a [coalition](../../../../../coalition-game-theory.md) are available. Company $i$ or $j$ alone has no requested [graph path](../../../../../path-in-a-graph.md); company $k$ carries two units of $B$–$C$ traffic. The pair $\{i,j\}$ carries one unit on each of $ABD,ACD$; the pair $\{i,k\}$ sends two units on $ABCD$ rather than selling them at the lower $B$–$C$ rate; and $\{j,k\}$ has only the two direct $B$–$C$ units. Therefore

$$
\begin{array}{c|rrrrrrr}
S&\{i\}&\{j\}&\{k\}&\{i,j\}&\{i,k\}&\{j,k\}&N\\ \hline
v(S)&0&0&8&12&12&8&22.
\end{array}
$$

Writing payments in thousands, all stable divisions of the revenue are exactly

$$
\boxed{\begin{gathered}
x_i+x_j+x_k=22,\qquad x_i,x_j\geq0,\quad x_k\geq8,\\
x_i+x_j\geq12,\quad x_i+x_k\geq12,\quad x_j+x_k\geq8.
\end{gathered}}
$$

Equivalently, $8\leq x_k\leq10$, $0\leq x_j\leq10$ and $x_i=22-x_j-x_k$. This is the entire [core](../../../../../core-game-theory.md), not just one acceptable allocation.

The [nucleolus](../../../../../nucleolus.md) minimizes in [lexicographic order](../../../../../lexicographic-order.md) the sorted decreasing [excesses of a coalition](../../../../../excess-of-a-coalition.md) $e(S,x)=v(S)-x(S)$ over [imputations](../../../../../imputation-in-a-coalitional-game.md). Empty and grand-coalition [coalition excesses](../../../../../excess-of-a-coalition.md) are fixed zeros and can be omitted. For the six other [coalitions](../../../../../coalition-game-theory.md), efficiency gives

$$
-x_i,\quad -x_j,\quad 8-x_k,\quad x_k-10,\quad x_j-10,\quad x_i-14.
$$

The two $k$-related [coalition excesses](../../../../../excess-of-a-coalition.md) sum to $-2$, so their [maximum](../../../../../maximum-of-a-subset-of-a-total-order.md) is at least $-1$. This bound is attainable, and attaining it forces $x_k=9$. All six [coalition excesses](../../../../../excess-of-a-coalition.md) are then at most $-1$ precisely when $1\leq x_j\leq9$ and $x_i=13-x_j$. The fixed pair of [coalition excesses](../../../../../excess-of-a-coalition.md) equals $-1$ throughout these first-stage minimizers.

Minimize the largest of the remaining [coalition excesses](../../../../../excess-of-a-coalition.md). They become $x_j-13,-x_j,x_j-10,-1-x_j$, whose [maximum](../../../../../maximum-of-a-subset-of-a-total-order.md) is $\max(-x_j,x_j-10)$. Its unique minimum is $-5$ at $x_j=5$. Hence $x_i=8$ and $x_k=9$. The sorted proper [coalition excesses](../../../../../excess-of-a-coalition.md) there are $(-1,-1,-5,-5,-6,-8)$, and

$$
\boxed{\text{the nucleolus pays }(\text{£}8000,\text{£}5000,\text{£}9000)
\text{ to }(i,j,k).}
$$

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 33](../../paper-33-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
