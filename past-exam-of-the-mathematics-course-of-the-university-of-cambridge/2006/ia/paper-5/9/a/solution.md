<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A graphical-component library can provide `protected void paintComponent(Graphics g)` as a subclass customization hook, as in `javax.swing.JComponent`. A subclass overrides it to draw its own contents while the library retains responsibility for the surrounding painting protocol. A [protected method in Java](../../../../../../protected-method-in-java.md) is accessible to code in the declaring package and to subclasses in other packages subject to the receiver restriction; it is not simply a public method and not exclusively subclass-visible.

**The benefit is controlled extensibility without exposing an ordinary client operation.** If the method were private, external subclasses could not override and reuse it as the intended hook. If it were public, arbitrary clients could call it outside the normal painting lifecycle and the library would have a wider public contract to maintain. Protected hooks still require documented invariants because subclass code participates in the implementation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [9](../../9.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
