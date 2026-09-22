<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We prove the result [algebraic partially ordered sets are continuous](../../../../../algebraic-partially-ordered-sets-are-continuous.md) directly from the definitions. First, $a\ll b$ implies $a\leq b$, by applying the [way-below relation](../../../../../way-below-relation.md) to the singleton [directed set](../../../../../directed-set.md) $\{b\}$. Also,

$$
a\ll b\leq c\quad\Longrightarrow\quad a\ll c:
$$

if $c\leq\sup D$, then $b\leq\sup D$, so the witness required for $a\ll b$ also works for $a\ll c$.

Fix $x$ and put

$$
K_x=\{k:k\leq x,\ k\ll k\},\qquad A_x=\{a:a\ll x\}.
$$

By algebraicity, $K_x$ is a [directed set](../../../../../directed-set.md) with [least upper bound](../../../../../least-upper-bound-in-a-partially-ordered-set.md) $x$. Every $k\in K_x$ satisfies $k\ll k\leq x$, hence $k\ll x$. Thus $K_x\subseteq A_x\subseteq\{a:a\leq x\}$.

To prove that $A_x$ is a [directed set](../../../../../directed-set.md), take $a,b\in A_x$. Applying $a\ll x$ and $b\ll x$ to $x=\sup K_x$ gives $k_a,k_b\in K_x$ such that $a\leq k_a$ and $b\leq k_b$. Directedness of $K_x$ gives $k\in K_x$ above both. Since $k\in A_x$, it is the required common [upper bound](../../../../../upper-bound-in-a-partially-ordered-set.md) inside $A_x$. With the usual nonempty convention, $A_x$ is nonempty since it contains $K_x$.

By directed completeness $A_x$ has a [least upper bound](../../../../../least-upper-bound-in-a-partially-ordered-set.md). The inclusions above give

$$
x=\sup K_x\leq\sup A_x\leq x,
$$

so

$$
\boxed{A_x\text{ is directed and }x=\sup A_x;\text{ hence the order is continuous}.}
$$

The same proof handles the paper's literal empty-set convention. If $K_x=\varnothing$, then $x=\sup\varnothing=\bot$, and the defining implication for $a\ll x$, applied to $D=K_x$, shows that $A_x$ must also be empty. Its [least upper bound](../../../../../least-upper-bound-in-a-partially-ordered-set.md) is again $x$. If $K_x$ is nonempty, the argument already given applies without change.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [6](../../6.md)
3. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
