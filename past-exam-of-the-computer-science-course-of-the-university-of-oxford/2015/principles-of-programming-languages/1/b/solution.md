<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the three [monad laws](../../../../../monad-laws.md) of the base [computational monad](../../../../../computational-monad.md). For left identity, at an arbitrary [program state](../../../../../program-state.md) $s$,

$$
\begin{aligned}
(\operatorname{result}(x)\triangleright f)\,s
&=r_m(x,s)\triangleright_m\bigl(\lambda(y,t).\,f(y)\,t\bigr)\\
&=f(x)\,s.
\end{aligned}
$$

The last step is the base left identity law. For right identity,

$$
\begin{aligned}
(p\triangleright\operatorname{result})\,s
&=(p\,s)\triangleright_m\bigl(\lambda(x,t).\,\operatorname{result}(x)\,t\bigr)\\
&=(p\,s)\triangleright_m\bigl(\lambda(x,t).\,r_m(x,t)\bigr)\\
&=(p\,s)\triangleright_m r_m=p\,s.
\end{aligned}
$$

The penultimate equality identifies the pair-destructuring [function](../../../../../function-split.md) with $r_m$; the last uses the base right identity law.

For [associativity](../../../../../associative-property.md), expand the two successive uses of sequencing and apply base [associativity](../../../../../associative-property.md):

$$
\begin{aligned}
((p\triangleright f)\triangleright g)\,s
&=\bigl((p\,s)\triangleright_m(\lambda(x,t).\,f(x)\,t)\bigr)
\triangleright_m(\lambda(y,u).\,g(y)\,u)\\
&=(p\,s)\triangleright_m\bigl(\lambda(x,t).\,
(f(x)\,t)\triangleright_m(\lambda(y,u).\,g(y)\,u)\bigr)\\
&=(p\,s)\triangleright_m\bigl(\lambda(x,t).\,(f(x)\triangleright g)\,t\bigr)\\
&=\bigl(p\triangleright(\lambda x.\,f(x)\triangleright g)\bigr)\,s.
\end{aligned}
$$

No [program state](../../../../../program-state.md) is duplicated or reset during these rearrangements: both sides pass $s$ to $p$, its output $t$ to $f$, and the output $u$ of $f$ to $g$. By [function extensionality](../../../../../function-extensionality.md),

$$
\boxed{\operatorname{result}(x)\triangleright f=f(x),\quad
p\triangleright\operatorname{result}=p,\quad
(p\triangleright f)\triangleright g=p\triangleright(\lambda x.\,f(x)\triangleright g).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Principles of programming languages](../../../principles-of-programming-languages-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
