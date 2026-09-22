<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [random forest](../../../../../../random-forest.md) fits each of its $500$ classification trees to an independent [bootstrap sample](../../../../../../bootstrap-sample.md) of the nine observations. At each node it draws `mtry=2` candidate coordinates; because the data have exactly two coordinates, both are available, and a CART impurity calculation chooses the split. The trees are grown deeply without ordinary cost-complexity pruning, and their [majority vote](../../../../../../majority-vote.md) is the forest prediction.

R reports an [out-of-bag error estimate](../../../../../../out-of-bag-error.md): an observation is predicted only by trees whose bootstrap samples omitted it. The [confusion matrix](../../../../../../confusion-matrix.md) says that class 1 has three correct and three incorrect out-of-bag predictions, while class 2 has one correct and two incorrect predictions. Hence the total out-of-bag error is $5/9$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
