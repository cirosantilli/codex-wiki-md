<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A generic class, interface or method in [Java](../../../../../../java-programming-language.md) is parameterized by one or more types. [Generics in Java](../../../../../../generics-in-java.md) allow one implementation of a collection or algorithm to be reused with different reference types while checking the allowed values and results statically. For example:
```
Vector<String> names = new Vector<String>();
names.add("Ada");
String first = names.get(0);

class Box<T> {
    private T value;
    public void put(T x) { value = x; }
    public T get() { return value; }
}
```
The type parameter is declared inside angle brackets, as in `Box<T>`, and supplied as a type argument, as in `Box<String>`. A generic method places its parameter list before its return type, for example `static <T> T identity(T x)`. Bounds such as `<T extends Number>` restrict type arguments, and wildcards such as `? extends Number` or `? super Integer` describe restricted views. Primitive values require wrapper types such as `Integer` rather than a type argument `int`. **Generics provide reusable code with compile-time checking of element types.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
