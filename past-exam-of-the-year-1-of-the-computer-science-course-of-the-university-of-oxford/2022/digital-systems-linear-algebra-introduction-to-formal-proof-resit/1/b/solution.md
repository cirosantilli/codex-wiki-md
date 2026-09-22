<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use an [explicit-stack depth-first tree traversal](../../../../../explicit-stack-depth-first-tree-traversal.md). Descend the left branch immediately and put each nonempty right subtree on a [stack](../../../../../stack-data-structure.md) for later. For the same node declarations as in the paper, an original [C programming language](../../../../../c-programming-language.md) implementation is:

```
int sum_iter(tree t)
{
    tree pending[32];
    unsigned top = 0;
    int total = 0;
    while (t != NULL || top != 0) {
        if (t == NULL) {
            t = pending[--top];
        } else {
            total += t->data;
            if (t->right != NULL)
                pending[top++] = t->right;
            t = t->left;
        }
    }
    return total;
}
```

The [loop invariant](../../../../../loop-invariant.md) says that the accumulated labels plus the sums of the current subtree and all pending subtrees equal the original tree sum, with the unvisited subtrees disjoint. Visiting a node adds its label and replaces its subtree by its two children. Popping merely changes which pending subtree is current. When both current and pending subtrees are absent, the invariant proves the result.

At most one unvisited right sibling is pending at each level of the current ancestor path. If depth means the number of nonempty nodes on a longest root-to-leaf path, depth at most 32 requires at most 31 pending right siblings. A 32-word array is therefore sufficient; it also covers the convention that depth counts at most 32 edges. The depth promise makes unchecked pushes valid here. For arbitrary input, a production implementation should check capacity rather than overwrite its frame.

A corresponding [Thumb instruction set](../../../../../thumb-instruction-set.md) implementation keeps the total in `r4`, the array base in `r5`, and its next-free address in `r6`:

```
.global sum_iter_asm
.thumb_func
sum_iter_asm:
    push {r4, r5, r6, lr}
    sub  sp, sp, #128        @ 32 pending pointers
    mov  r5, sp              @ base of pending array
    mov  r6, sp              @ empty stack: next-free equals base
    movs r4, #0
.Lvisit:
    cmp  r0, #0
    beq  .Ltake_pending
    ldr  r1, [r0, #0]
    adds r4, r4, r1          @ consume this node's label
    ldr  r1, [r0, #8]
    cmp  r1, #0
    beq  .Lleft
    str  r1, [r6, #0]        @ defer the nonempty right subtree
    adds r6, r6, #4
.Lleft:
    ldr  r0, [r0, #4]        @ continue down the left branch
    b    .Lvisit
.Ltake_pending:
    cmp  r6, r5
    beq  .Ldone
    subs r6, r6, #4
    ldr  r0, [r6, #0]
    b    .Lvisit
.Ldone:
    movs r0, r4
    add  sp, sp, #128
    pop  {r4, r5, r6, pc}
```

The [stack pointer](../../../../../stack-pointer.md) stays fixed while the array is used; `r6` is a separate cursor inside that array. All [callee-saved registers](../../../../../callee-saved-register.md) touched by the function are restored. **Each nonempty node contributes its label exactly once.** As in part (a), require that every partial total fits the signed result type; a representable final answer alone does not prevent overflow in a different summation order.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof resit](../../../digital-systems-linear-algebra-introduction-to-formal-proof-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
