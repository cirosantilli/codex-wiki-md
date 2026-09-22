<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

A [regular expression](../../../../../regular-expression.md) is built from $\emptyset$, $\epsilon$, and alphabet symbols using union, concatenation, and Kleene star; its language is defined by applying the corresponding set operations recursively. A [deterministic finite automaton](../../../../../deterministic-finite-automaton.md) is a tuple $(Q,\Sigma,\delta,q_0,F)$ and accepts

$$
L(D)=\{w:\widehat\delta(q_0,w)\in F\}.
$$

[Kleene theorem](../../../../../kleene-theorem.md) says that the languages denoted by regular expressions are exactly those accepted by finite automata.

Regular languages are closed under finite union, using a product automaton or nondeterministic choice, and under finite intersection, using the product automaton with accepting set $F_L\times F_M$.

They are not closed under countable unions or intersections. Every language over a finite alphabet is a countable union of singleton languages, each regular, so a nonregular language such as $\{a^nb^n:n\geq0\}$ is a counterexample. It is also

$$
\bigcap_{w\notin L}(\Sigma^*\setminus\{w\}),
$$

a countable intersection of regular languages, giving the second counterexample.

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
