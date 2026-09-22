<h1 id="5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assuming `p` is an ordinary total Boolean predicate, replace success by `true` and the search's failure exception by `false`:
```
fun gordonPlain p Lf = true
  | gordonPlain p (Br (x, left, right)) =
      p x andalso
      (gordonPlain p left orelse gordonPlain p right);
```
The [Standard ML](../../../../../../../standard-ml.md) handler in the printed function belongs to the `else` expression: it tries the left subtree and, only if that search raises `Blair`, tries the right. It does not catch a failing label test at the current node. This scope follows the [Standard ML grammar, Appendix B](https://smlfamily.github.io/sml97-defn.pdf). Short-circuit `andalso` rejects the current label before visiting either child; short-circuit `orelse` visits the right child only after the left search fails. [Structural induction](../../../../../../../structural-induction.md) on the [binary tree](../../../../../../../binary-tree.md) proves that `tony` returns `true` exactly when `gordonPlain` does, and otherwise raises the exception converted by `gordon` to `false`. **The exception-free test is the root predicate conjoined with the disjunction of the two subtree tests.**

The total-predicate assumption matters: if `p` itself raises `Blair`, the original handler can catch it, whereas an implementation with no [exception handling](../../../../../../../exception-handling.md) cannot in general convert that event to a Boolean result. The displayed replacement implements the intended Boolean tree property, not an exception-catching wrapper for arbitrary exceptional predicates.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Ia](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
