<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Interpret a [function collision](../../../../../../function-collision.md) as two distinct inputs with equal outputs. Without distinctness the request is vacuous, since an input paired with itself always qualifies. Set $m=\lceil N^{1/3}\rceil$ (handling small $N$ by direct queries), choose a known set $A$ of size $m$, and query all its inputs. Store a classical table of their outputs and corresponding inputs. If this table contains a [function collision](../../../../../../function-collision.md), return it immediately.

Otherwise the table contains $m$ distinct outputs. Because $g$ is exactly two-to-one, each $a\in A$ has exactly one partner in $B$, the known complement of $A$. None lies in $A$, and different table outputs have different partners. Thus exactly $m$ inputs in $B$, of size $L=N-m$, satisfy the known-table membership predicate

$$
h(b)=1\quad\Longleftrightarrow\quad g(b)\in\{g(a):a\in A\}.
$$

Build a [marked-state phase oracle](../../../../../../marked-state-phase-oracle.md) for this predicate by a [compute-phase-uncompute construction](../../../../../../compute-phase-uncompute-construction.md): use $U_g$ on a clean answer [quantum register](../../../../../../quantum-register.md), reversibly compare its output against the classical table, apply the conditional minus sign, undo the comparison, and apply $U_g$ again. Since the answer operation is bitwise [exclusive or](../../../../../../exclusive-or.md), $U_g^{-1}=U_g$. All workspace returns to zero, and each phase query costs two calls to $U_g$.

Perform [known-subset Grover search](../../../../../../known-subset-grover-search.md) in the [span](../../../../../../linear-span.md) of the [computational basis](../../../../../../computational-basis.md) states labelled by $B$, starting in their [uniform superposition state](../../../../../../uniform-superposition-state.md). Reflection about this known state uses no $U_g$ queries; choosing $A$ as an initial interval makes $B$ a known interval that can also be encoded by its own $L$ labels. Its marked fraction is $m/L$, so the previous [Grover rotation angle](../../../../../../grover-rotation-angle.md) analysis uses $O(\sqrt{L/m})$ phase queries. On measuring $b$, one further $U_g$ query checks the output and retrieves its partner $a$ from the table. The inputs are distinct because the two sets are disjoint.

Consequently the [quantum query complexity](../../../../../../quantum-query-complexity.md) is

$$
\boxed{m+O\!\left(\sqrt{\frac{N-m}{m}}\right)+1=O(N^{1/3}).}
$$

For large $N$, rounding the optimal [Grover search algorithm](../../../../../../grover-s-algorithm.md) iteration count gives success at least $1-m/(N-m)>1/2$. An internal table [function collision](../../../../../../function-collision.md) already gives certain success. The balance $m\asymp\sqrt{N/m}$ explains the cube-root choice. This is the [Brassard–Høyer–Tapp collision algorithm](../../../../../../brassard-hoyer-tapp-collision-algorithm.md): its table uses $O(m\log N)$ classical bits. The bound counts calls to $U_g$, as requested; it does not charge table lookup and its reversible implementation as constant-time gates, or claim an overall polynomial time in $\log N$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
