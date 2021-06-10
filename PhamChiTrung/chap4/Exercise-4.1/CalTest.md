* Here the test case CalTest:

```java
class CalcTest {

    @BeforeEachTesting
    void setUp() {

    }

    @Testing1
    void testSubtract() {
        int a, b;
        a = 4;
        b = 2;
        assertEquals(2, Calc.subtract(a, b));
    }

    @Testing2
    void testMultiply() {
        int a, b;
        a = 4;
        b = 2;
        assertEquals(8, Calc.multiply(a, b));
    }

    @Testing3
    void testDivide() {
        int a, b;
        a = 4;
        b = 2;
        assertEquals(2, Calc.divide(a, b));
    }

    @AfterEachTesting
    void tearDown() {
    }
}
```
