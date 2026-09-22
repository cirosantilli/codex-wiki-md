<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Sum net outflow over all [vertices](../../../../../vertex-graph-theory.md) in the source side $S$. An internal [directed edge](../../../../../directed-edge.md) occurs once positively and once negatively, so it cancels. All internal [vertices](../../../../../vertex-graph-theory.md) have zero net outflow by [flow conservation](../../../../../flow-conservation.md), and the sink is outside $S$. Therefore

$$
|f|=\sum_{\substack{(u,v)\in E\\u\in S,\,v\notin S}}f(u,v)-\sum_{\substack{(u,v)\in E\\u\notin S,\,v\in S}}f(u,v).
$$

The second [sum](../../../../../sum.md) is nonnegative, while every term in the first satisfies its [capacity constraint](../../../../../capacity-constraint.md). Consequently,

$$
\boxed{|f|\leq\sum_{\substack{(u,v)\in E\\u\in S,\,v\notin S}}c(u,v)=c(S,V\setminus S).}
$$

This is direct accounting from [flow conservation](../../../../../flow-conservation.md); it does not invoke the [max-flow min-cut theorem](../../../../../max-flow-min-cut-theorem.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Algorithms](../../../algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
