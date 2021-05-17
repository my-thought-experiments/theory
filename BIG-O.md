# Big O Notation

Simplified analysis of an algorithm's efficiency.

## Type of measurement

1. Worst-case
2. Best-case
3. Average-case

## General rules

1. Igore constants.

    For eg. 5n --> O(n)

2. Certain teams dominate others

    For eg.
    O(1) < O(Log n) < O(n) < O(n Log n) < O(n^2) < O(2^n) < O(n!)

    **In Table form:**
    | Teams | Notation | Comments |
    |:---|:---|:---|
    | Excellent | O(1) | Constant |
    | Good | O(Log n) | Logarithmic |
    | Fair | O(n) | Linear |
    | Bad | O(n Log n) | 
    | Horrible | O(n^2) / O(2^n) | Exponential |
    |  | O(n!) | Factorial |

### Time

Rules

  1. Find the fastest growing term
  2. Take out the co-efficient

1. **Constant time**: Independent of input size, n. Hence, O(1)

    For eg.

    ```
    T = c = 0.343 = 0.343 * 1 = O(1)
    ```

    ```
    x = 5 + (15 * 20) // O(1)
    ```

    ```
    x = 5 + (15 * 20)
    y = 15 - 2
    print x + y // O(1)
    ```
    Total time = O(1) + O(1) + O(1) = O(1)

2. **Logarithmic time**: O(Log n)

3. **Linear time**: n * O(1) = O(n)

    For eg.

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

4. **Quadratic time**: O(n^2)

    For eg.

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

* [Desmos](https:/www.desmos.com)
