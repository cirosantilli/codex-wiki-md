<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [continuation](../../../../../continuation-computer-science.md) receives both the computed value and the current [computer memory](../../../../../computer-memory-split.md). Therefore return invokes it with unchanged [computer memory](../../../../../computer-memory-split.md), while sequencing installs a [continuation](../../../../../continuation-computer-science.md) that passes the produced value and updated [computer memory](../../../../../computer-memory-split.md) to the next computation:

```
result :: a -> M a
result x k s = k x s

bind :: M a -> (a -> M b) -> M b
bind p f k s = p (\x s' -> f x k s') s
```

For left identity, expand the two definitions:

$$
(\operatorname{result}(x)\triangleright f)\,k\,s
=(\lambda y\,t.\,f(y)\,k\,t)\,x\,s=f(x)\,k\,s.
$$

For right identity,

$$
(p\triangleright\operatorname{result})\,k\,s
=p(\lambda x\,t.\,\operatorname{result}(x)\,k\,t)\,s
=p(\lambda x\,t.\,k\,x\,t)\,s=p\,k\,s.
$$

For [associativity](../../../../../associative-property.md), both groupings reduce to the same expression:

$$
\begin{aligned}
((p\triangleright f)\triangleright g)\,k\,s
&=p\bigl(\lambda x\,t.\,f(x)(\lambda y\,u.\,g(y)\,k\,u)\,t\bigr)\,s,\\
\bigl(p\triangleright(\lambda x.\,f(x)\triangleright g)\bigr)\,k\,s
&=p\bigl(\lambda x\,t.\,f(x)(\lambda y\,u.\,g(y)\,k\,u)\,t\bigr)\,s.
\end{aligned}
$$

By [function extensionality](../../../../../function-extensionality.md), these establish all three [monad laws](../../../../../monad-laws.md):

$$
\boxed{\operatorname{result}(x)\triangleright f=f(x),\qquad
p\triangleright\operatorname{result}=p,\qquad
(p\triangleright f)\triangleright g=p\triangleright(\lambda x.\,f(x)\triangleright g).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Principles of programming languages](../../../principles-of-programming-languages-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
