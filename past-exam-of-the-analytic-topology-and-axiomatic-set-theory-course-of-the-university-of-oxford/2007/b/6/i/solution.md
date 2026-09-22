<h1 id="b/6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [transitive closure](../../../../../transitive-closure.md) $\operatorname{TC}(a)$ is the least [transitive set](../../../../../transitive-set.md) containing $a$ as a subset. Put $a_0=a$, $a_{n+1}=\bigcup a_n$ and define

$$
\boxed{\operatorname{TC}(a)=\bigcup_{n<\omega}a_n.}
$$

Recursion and [Replacement](../../../../../axiom-schema-of-replacement.md) give the set of iterates, and Union gives its union. It contains $a=a_0$ as a subset. If $u\in v\in\operatorname{TC}(a)$, then $v\in a_n$ for some $n$, so $u\in a_{n+1}\subseteq\operatorname{TC}(a)$; hence it is transitive.

If $T$ is transitive with $a\subseteq T$, induction gives $a_n\subseteq T$ for every $n$, because $\bigcup T\subseteq T$. Therefore $\operatorname{TC}(a)\subseteq T$. This proves minimality and uniqueness. If the alternative convention asks for the least [transitive set](../../../../../transitive-set.md) containing $a$ as an element, that set is $\operatorname{TC}(\{a\})$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the analytic topology and axiomatic set theory course of the University of Oxford](../../../../split.md)
6. [Analytic topology and axiomatic set theory course of the University of Oxford](../../../../../analytic-topology-and-axiomatic-set-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
