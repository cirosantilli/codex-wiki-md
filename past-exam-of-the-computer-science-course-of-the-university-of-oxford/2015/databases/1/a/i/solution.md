<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First use [relational selection](../../../../../../relational-selection.md) to keep the Saab cars, then a [natural join](../../../../../../natural-join.md) to find their sales, and finally a [relational join](../../../../../../relational-join.md) to identify the corresponding salespeople. A [relational projection](../../../../../../relational-projection.md) gives

$$
\boxed{\pi_{\mathsf{name}}\!\left(P\bowtie_{\mathsf{empid=salespersonid}}\left(S\bowtie\sigma_{\mathsf{make}=\text{Saab}}C\right)\right).}
$$

The [foreign keys](../../../../../../foreign-key.md) ensure that every sale has the referenced car and salesperson. Several qualifying sales by the same person produce just one occurrence of their name under [set semantics](../../../../../../set-semantics.md). Two distinct people with the same name also yield that name only once: this is the requested [relational projection](../../../../../../relational-projection.md) onto names.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Databases](../../../../databases-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
