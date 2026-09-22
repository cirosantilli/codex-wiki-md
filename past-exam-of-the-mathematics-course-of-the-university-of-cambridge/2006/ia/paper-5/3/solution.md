<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Extract one four-bit digit at a time, beginning at the most significant end of the [Java](../../../../../java-programming-language.md) `int`. A lookup string supplies characters, but no library performs the conversion:
```
java
static String toHex(int value) {
    String digits = "0123456789abcdef";
    String answer = "";
    boolean started = false;
    for (int shift = 28; shift >= 0; shift -= 4) {
        int digit = (value >>> shift) & 15;
        if (started || digit != 0 || shift == 0) {
            answer = answer + digits.charAt(digit);
            started = true;
        }
    }
    return answer;
}
```
The logical right [bit shift](../../../../../bit-shift.md) `>>>` inserts zeros, and the [bit mask](../../../../../bit-mask.md) `15` retains exactly the low four bits of the shifted word. Each emitted character is therefore the corresponding [hexadecimal](../../../../../hexadecimal.md) digit. The `started` flag suppresses leading zero digits; the `shift == 0` exception makes zero produce **`"0"`**, rather than an empty string.

A negative [Java](../../../../../java-programming-language.md) integer uses [two's complement](../../../../../two-s-complement.md). Its top bit is set, so the first extracted digit is between eight and fifteen and all eight digits are emitted. We interpret its original 32-bit pattern, without taking an absolute value or negating a potentially unnegatable minimum integer. In particular, **`toHex(19)` returns `"13"`, `toHex(-1)` returns `"ffffffff"`, and `toHex(Integer.MIN_VALUE)` returns `"80000000"`.** There are exactly eight iterations, so for this fixed word size the [time complexity](../../../../../time-complexity.md) is constant.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 5](../../paper-5-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
