<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Print separators before all but the first term, so there is neither a leading nor a trailing plus sign:
```
def printRat(num: Int, den: Int): Unit = {
  print(num.toString + "/" + den.toString)
}

def printEgypt(e: Array[Int]): Unit = {
  if (e.isEmpty) print("0")
  var i = 0
  while (i < e.length) {
    if (i > 0) print(" + ")
    print("1/" + e(i).toString)
    i += 1
  }
}
```
The [loop invariant](../../../../../loop-invariant.md) says that exactly the first $i$ [unit fractions](../../../../../unit-fraction.md) have been printed in order, separated by ` + `, with no trailing separator. The [loop variant](../../../../../loop-variant.md) is $e.length-i$. The empty [array](../../../../../array-data-structure.md) is displayed as zero. Since $5/7-1/2=3/14$ and $3/14-1/5=1/70$, **the output is `5/7 = 1/2 + 1/5 + 1/70`**. The source's earlier example with middle denominator $4$ and final denominator $70$ contains the arithmetic typo; its final printing example is correct. Indeed $1/2+1/4>5/7$, so no positive final term could repair that particular prefix. The printing routine reports the generated terms rather than imposing a particular expansion.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Imperative programming resit](../../../imperative-programming-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
