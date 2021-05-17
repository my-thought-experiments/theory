# Analysis of algorithms

A language and metric to describe the efficiency of algorithm.

**Asymptotic Analysis**

* The main idea of asymptotic analysis is to have a measure of the efficiency of algorithms that
don't depend on machine specific constants and doesn't require algorithms to be implemented
and time taken by programs to be compared.

* Asymptotic notations are mathematical tools to represent Time and Space Complexity.

**Notations**

1. Big O

* Useful for evaluating worst case performance of an algorithm.
* At most upper bound.

2. Big Omega Ω

* Useful for evaluating best case performance of an algorithm.
* At lease lower bound.

3. Big Theta Θ

* Useful for evaluating average case performance of an algorithm.
* Exact time

## Time Complexity

**Rules**

1. Find the fastest growing term.

    Example
    ```
    O(1) < O(Log n) < O(n) < O(n Log n) < O(n^2) < O(2^n) < O(n!)
    ```

2. Take out the co-efficient/constants.

    Example
    ```
    5n --> O(n)
    ```

### Constant time

Independent of input size (n). Hence, O(1)

Example
```
T = c = 0.343 = 0.343 * 1 --> O(1)
```

```
x = 5 + (15 * 20) --> O(1)
```

```
x = 5 + (15 * 20) --> O(1)
y = 15 - 2 --> O(1)
print x + y --> O(1)
```
Total time = O(1) + O(1) + O(1) = O(1)

### Logarithmic time

O(Log n)

### Linear time

n * O(1) = O(n)

    Example

    ```
    T = an + b = O(n)
    ```

    ```
    for x in rage (0, n): // O(n)
      print x; // O(1)
    ```

    ```
    x = 5 + (15 * 20) // O(1)
    for x in rage (0, n): // O(n)
      print x;
    ```
    Total time = O(1) + O(n) = O(n)

## Quadratic time

O(n^2)

    Example

    ```
    T = cn^2 + dn + e = O(n^2)
    ```

    ```
    for x in rage (0, n): // O(n)
      for y in rage (0, n): // O(n)
        print x * y // O(1)
    ```
    Total time = O(n^2) + O(1) = O(n^2)

    Understand **Total time**

    ```
    // O(1)
    x = 5 + (15 * 20) // O(1)

    // O(n)
    for x in rage (0, n): // O(n)
      print x;

    // O(n^2)
    for x in rage (0, n): // O(n)
      for y in rage (0, n): // O(n)
        print x * y // O(1)
    ```
    Total time = O(1) + O(n) + O(n^2) = O(n^2)


    ```
    if x > 0:
      // O(1)
    else if x < 0:
      // O(Log n)
    else:
      // O(n^2)
    ```
    Total time = O(1) + O(Log n) + O(n^2) = O(n^2)


**From Slowest to Fastest Growing**

| Function Type | | Example |
|:---|:---|:---|
| Constant | O(1) | 5, 25, 2500 |
| Logarithmic | O(Log n)| Log n |
| Linear | O(n) | 5n, 25n, 2500n |
| Linearithmic | O(n Log n) | n Log n |
| Polynomial | O(n^2) | 5n^2, 25n^4, 2500n^8 |
| Exponential | O(c^n) | 5^n, 25^25000n |
| Factorial | O(n!) | |

Where n = number of inputs and c = constant

## Algorithms

<table>
  <thead>
    <tr>
      <th rowspan="2">Algorithm</th>
      <th colspan="3">Time Complexity</th>
    </tr>
    <tr>
      <th>Best</th>
      <th>Average</th>
      <th>Worst</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td colspan="4"><strong>Searching</strong></td>
    </tr>
    <tr>
      <td>Binary search</td>
      <td>O(1)</td>
      <td>O(Log n)</td>
      <td>O(Log n)</td>
    </tr>
    <tr>
      <td>Sequential/Linear search</td>
      <td>O(1)</td>
      <td>O(n)</td>
      <td>O(n)</td>
    </tr>
    <tr>
      <td colspan="4"><strong>Sorting</strong></td>
    </tr>
    <tr>
      <td>Bubble sort</td>
      <td>O(n)</td>
      <td>O(n^2)</td>
      <td>O(n^2)</td>
    </tr>
    <tr>
      <td>Selection sort</td>
      <td>O(n^2)</td>
      <td>O(n^2)</td>
      <td>O(n^2)</td>
    </tr>
    <tr>
      <td>Insertion sort</td>
      <td>O(n)</td>
      <td>O(n^2)</td>
      <td>O(n^2)</td>
    </tr>
    <tr>
      <td>Merge sort</td>
      <td>O(n Log n)</td>
      <td>O(n Log n)</td>
      <td>O(n Log n)</td>
    </tr>
    <tr>
      <td>Quick sort</td>
      <td>O(n Log n)</td>
      <td>O(n Log n)</td>
      <td>O(n^2)</td>
    </tr>
    <tr>
      <td>Heap sort</td>
      <td>O(n Log n)</td>
      <td>O(n Log n)</td>
      <td>O(n Log n)</td>
    </tr>
  </tbody>
</table>


## References

* [https://www.youtube.com/watch?v=ei-A_wy5Yxw&ab_channel=profbillbyrne](https://www.youtube.com/watch?v=ei-A_wy5Yxw&ab_channel=profbillbyrne)
* [Desmos](https:/www.desmos.com)
