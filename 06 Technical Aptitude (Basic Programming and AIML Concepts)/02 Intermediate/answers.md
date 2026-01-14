# Answers - Technical Aptitude (Intermediate Level)

## Programming Fundamentals (1–20)

1. **Solution**:
   In `printf`, arguments are evaluated right-to-left. `++x` increments `x` to 6, then `x++` uses 6 and increments `x` to 7. Output: `6 6`.  
   **Answer**: 6 6


2. **Solution**:
   `y = x` creates a reference to the same list. Modifying `y[0]` changes `x`. Output: `[4, 2, 3]`.  
   **Answer**: [4, 2, 3]


3. **Solution**:
   `concat` creates a new string `"hello world"`. Output: `hello world`.  
   **Answer**: hello world


4. **Solution**:
   Ternary operator: `x > 5` is true, so prints `x = 10`.  
   **Answer**: 10


5. **Solution**:
   Python passes integers by value. `x` inside `f` is local. Output: `5`.  
   **Answer**: 5


6. **Solution**:
   `x << 2` left-shifts `10` (binary `1010`) to `101000` (40).  
   **Answer**: 40


7. **Solution**:
   `arr.length - 1 = 2`. `arr[2] = 3`.  
   **Answer**: 3


8. **Solution**:
   `update` modifies key `2` to `'c'`. Output: `{1: 'a', 2: 'c'}`.  
   **Answer**: {1: 'a', 2: 'c'}


9. **Solution**:
   Loop: `x = 5 * 2 * 2 * 2 = 40`.  
   **Answer**: 40


10. **Solution**:
    `a ^ b`: `7` (binary `111`) XOR `3` (binary `011`) = `100` (4).  
    **Answer**: 4


11. **Solution**:
    Slicing `[1:3]` includes indices 1 to 2: `[2, 3]`.  
    **Answer**: [2, 3]


12. **Solution**:
    `x & (x - 1)` clears the least significant set bit. `15` (binary `1111`) & `14` (binary `1110`) = `1110` (14).  
    **Answer**: 14


13. **Solution**:
    `reverse` reverses the string: `"abc"` becomes `"cba"`.  
    **Answer**: cba


14. **Solution**:
    Lambda function doubles input: `3 * 2 = 6`.  
    **Answer**: 6


15. **Solution**:
    `~x` inverts bits of `5` (binary `00000101`) to `11111010` (two’s complement, -6).  
    **Answer**: -6


16. **Solution**:
    `x >> 1` right-shifts `8` (binary `1000`) to `0100` (4).  
    **Answer**: 4


17. **Solution**:
    `copy()` creates a shallow copy. Modifying `y` doesn’t affect `x`. Output: `[1, 2]`.  
    **Answer**: [1, 2]


18. **Solution**:
    `x << 1 = 3 * 2 = 6`. `x >> 1 = 3 / 2 = 1`. `6 + 1 = 7`.  
    **Answer**: 7


19. **Solution**:
    `*(arr + 1)` accesses `arr[1] = 2`.  
    **Answer**: 2


20. **Solution**:
    `map` applies square function: `[1², 2², 3²] = [1, 4, 9]`.  
    **Answer**: [1, 4, 9]


## Data Structures (21–40)

21. **Solution**:
    Traverse to the end to update the pointer: O(n).  
    **Answer**: O(n)


22. **Solution**:
    Stack (LIFO): Push `1, 2, 3`. Pop removes `3`, then `2`. Stack: `[1]`.  
    **Answer**: [1]


23. **Solution**:
    Update prev/next pointers of adjacent nodes: O(1).  
    **Answer**: O(1)


24. **Solution**:
    Queue (FIFO): Enqueue `1, 2, 3`. Dequeue removes `1`. Enqueue `4`. Dequeue removes `2`. Front: `3`.  
    **Answer**: 3


25. **Solution**:
    Worst case (skewed tree) resembles a linked list: O(n).  
    **Answer**: O(n)


26. **Solution**:
    Deque: Append `3`, popleft removes `1`. Deque: `[2, 3]`.  
    **Answer**: deque([2, 3])


27. **Solution**:
    Insert at bottom, bubble up to restore heap property: O(log n).  
    **Answer**: O(log n)


28. **Solution**:
    Recursively visit all nodes: O(n).  
    **Answer**: O(n)


29. **Solution**:
    `pop('a')` removes key `'a'`. Output: `{'b': 2}`.  
    **Answer**: {'b': 2}


30. **Solution**:
    Replace root with last element, bubble down: O(log n).  
    **Answer**: O(log n)


31. **Solution**:
    Update pointers of given and next node: O(1).  
    **Answer**: O(1)


32. **Solution**:
    `discard(2)` removes `2`. Output: `{1, 3}`.  
    **Answer**: {1, 3}


33. **Solution**:
    Traverse to the leftmost node: O(h), where h is height (O(log n) if balanced).  
    **Answer**: O(log n) (balanced)


34. **Solution**:
    Recursion stack uses O(h), where h is height (O(log n) if balanced).  
    **Answer**: O(log n) (balanced)


35. **Solution**:
    Append `5` to `x[0]`. Output: `[[1, 2, 5], [3, 4]]`.  
    **Answer**: [[1, 2, 5], [3, 4]]


36. **Solution**:
    Visit all nodes using a queue: O(n).  
    **Answer**: O(n)


37. **Solution**:
    Average chain length = n/m. Search: O(n/m). If m ≈ n, O(1).  
    **Answer**: O(1) (assuming m ≈ n)


38. **Solution**:
    `Counter` counts occurrences. `c[2]` = 2 (two `2`s).  
    **Answer**: 2


39. **Solution**:
    Compute height of each subtree, check difference: O(n).  
    **Answer**: O(n)


40. **Solution**:
    Stack: Push `1, 2, 3`. Pop removes `3`. Push `4`. Pop removes `4`. Top: `2`.  
    **Answer**: 2


## Algorithms (41–60)

41. **Solution**:
    Divide and merge: O(n log n).  
    **Answer**: O(n log n)


42. **Solution**:
    Binary search finds `3` at index `2`.  
    **Answer**: 2


43. **Solution**:
    Recursion stack: O(log n) average, O(n) worst case.  
    **Answer**: O(log n) (average)


44. **Solution**:
    Euclidean algorithm: `gcd(48, 18) = gcd(18, 12) = gcd(12, 6) = gcd(6, 0) = 6`.  
    **Answer**: 6


45. **Solution**:
    Using a hash set: O(n). Without hash set: O(n²).  
    **Answer**: O(n) (with hash set)


46. **Solution**:
    `sort()` sorts in-place: `[1, 2, 4, 5]`.  
    **Answer**: [1, 2, 4, 5]


47. **Solution**:
    Priority queue operations: O((V + E) log V).  
    **Answer**: O((V + E) log V)


48. **Solution**:
    `rotate` shifts left by 1: `[2, 3, 1]`. First element: `2`.  
    **Answer**: 2


49. **Solution**:
    Compare and shift: O(n²).  
    **Answer**: O(n²)


50. **Solution**:
    List comprehension filters even numbers: `[2, 4]`.  
    **Answer**: [2, 4]


51. **Solution**:
    Compare characters from both ends: O(n).  
    **Answer**: O(n)


52. **Solution**:
    `fib(5) = fib(4) + fib(3) = (fib(3) + fib(2)) + (fib(2) + fib(1)) = (2 + 1) + (1 + 1) = 5`.  
    **Answer**: 5


53. **Solution**:
    Extra array for merging: O(n).  
    **Answer**: O(n)


54. **Solution**:
    `reversed` reverses string: `"olleh"`.  
    **Answer**: olleh


55. **Solution**:
    Compare characters across strings: O(n * m).  
    **Answer**: O(n * m)


56. **Solution**:
    `*(p + 2)` accesses `arr[2] = 3`.  
    **Answer**: 3


57. **Solution**:
    Create count array and output: O(n + k).  
    **Answer**: O(n + k)


58. **Solution**:
    `set(x)` removes duplicates, `list` converts back: `[1, 2, 3]`.  
    **Answer**: [1, 2, 3]


59. **Solution**:
    Floyd’s cycle-finding algorithm (two pointers): O(n).  
    **Answer**: O(n)


60. **Solution**:
    `qsort` sorts array: `[1, 3, 4]`. First element: `1`.  
    **Answer**: 1


## Database Basics (61–70)

61. **Solution**:
    Retrieves `name` and `salary` for `department = 'IT'`, sorted by `salary` in descending order.  
    **Answer**: IT employees sorted by salary (highest first)


62. **Solution**:
    Combines rows from `orders` and `customers` where `customer_id` matches `id`.  
    **Answer**: Joins orders with customer details


63. **Solution**:
    Counts employees per `department`.  
    **Answer**: Department-wise employee counts


64. **Solution**:
    Ensures values in a column match values in another table’s primary key.  
    **Answer**: Referential integrity


65. **Solution**:
    Retrieves `product_name` where `price` is 50 to 100 (inclusive).  
    **Answer**: Products priced 50–100


66. **Solution**:
    Returns unique `city` values from `customers`.  
    **Answer**: Unique cities


67. **Solution**:
    Retrieves `name` of students with `marks` above the average.  
    **Answer**: Students with above-average marks


68. **Solution**:
    Adds an `email` column to `employees` table.  
    **Answer**: Adds email column


69. **Solution**:
    Includes all `orders`, with matching `customer_name` or NULL if no match.  
    **Answer**: All orders with customer names (or NULL)


70. **Solution**:
    Creates an index on `name` column to speed up queries.  
    **Answer**: Improves query performance


## Computer Networks (71–80)

71. **Solution**:
    Provides a framework for network communication with seven layers.  
    **Answer**: Standardizes network communication


72. **Solution**:
    Network layer (Layer 3) manages routing.  
    **Answer**: Network layer


73. **Solution**:
    HTTPS uses port 443 for secure communication.  
    **Answer**: 443


74. **Solution**:
    Maps private IP addresses to a public IP for internet access.  
    **Answer**: IP address mapping


75. **Solution**:
    Hub broadcasts data to all ports; switch forwards data to specific devices.  
    **Answer**: Hub: broadcasts, Switch: targeted


76. **Solution**:
    Uniquely identifies a device at the data link layer.  
    **Answer**: Device identification


77. **Solution**:
    SYN, SYN-ACK, ACK to establish a connection.  
    **Answer**: Connection establishment


78. **Solution**:
    Handles error messages and diagnostics (e.g., ping).  
    **Answer**: Error reporting


79. **Solution**:
    `/28` (240 = 11110000) has 2⁴ = 16 addresses (14 hosts, 1 network, 1 broadcast).  
    **Answer**: 14


80. **Solution**:
    Border Gateway Protocol routes data between autonomous systems.  
    **Answer**: Inter-domain routing


## Operating Systems (81–90)

81. **Solution**:
    Preemptive: CPU can interrupt a process; Non-preemptive: process runs to completion.  
    **Answer**: Preemptive: interruptible, Non-preemptive: uninterruptible


82. **Solution**:
    Synchronization tool to control access to shared resources.  
    **Answer**: Synchronization mechanism


83. **Solution**:
    Divides memory into fixed-size pages to simplify allocation.  
    **Answer**: Memory allocation


84. **Solution**:
    Process: independent program with own memory; Thread: lightweight, shares process memory.  
    **Answer**: Process: isolated, Thread: shared memory


85. **Solution**:
    Disk space used to store inactive pages when RAM is full.  
    **Answer**: Extends virtual memory


86. **Solution**:
    Saves current process state and loads another to switch execution.  
    **Answer**: Process switching


87. **Solution**:
    Replaces the least recently used page to minimize page faults.  
    **Answer**: Optimizes page replacement


88. **Solution**:
    Occurs when multiple processes access shared data concurrently, leading to unpredictable results.  
    **Answer**: Concurrent access issue


89. **Solution**:
    Tracks file locations on disk.  
    **Answer**: File location tracking


90. **Solution**:
    Ensures mutual exclusion to prevent concurrent access to critical sections.  
    **Answer**: Mutual exclusion


## AI/ML Foundations (91–100)

91. **Solution**:
    Classification predicts discrete labels; regression predicts continuous values.  
    **Answer**: Classification: labels, Regression: values


92. **Solution**:
    Splits data into multiple folds to evaluate model performance robustly.  
    **Answer**: Robust model evaluation


93. **Solution**:
    High bias: underfitting; high variance: overfitting. Balance minimizes error.  
    **Answer**: Balances underfitting and overfitting


94. **Solution**:
    Controls step size for parameter updates during optimization.  
    **Answer**: Step size control


95. **Solution**:
    Adds penalty to model complexity to prevent overfitting.  
    **Answer**: Prevents overfitting


96. **Solution**:
    Perceptron: single-layer; MLP: multiple layers for non-linear problems.  
    **Answer**: Perceptron: single, MLP: multiple layers


97. **Solution**:
    Converts logits to probabilities for multi-class classification.  
    **Answer**: Probability conversion


98. **Solution**:
    Number of neighbors considered for prediction.  
    **Answer**: Neighbor count


99. **Solution**:
    Bagging: parallel ensembles (e.g., Random Forest); Boosting: sequential, corrects errors (e.g., AdaBoost).  
    **Answer**: Bagging: parallel, Boosting: sequential


100. **Solution**:
     Reduces dimensionality by projecting data onto principal components.  
     **Answer**: Dimensionality reduction
