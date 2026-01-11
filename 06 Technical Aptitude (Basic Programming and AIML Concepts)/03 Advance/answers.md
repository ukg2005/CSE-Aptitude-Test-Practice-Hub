# Answers - Technical Aptitude (Advanced Level)

## Programming Fundamentals (1–20)

1. **Solution**:
   `p` points to `x`. `*p += 2` modifies `x` to `5 + 2 = 7`. Both `x` and `*p` access the same memory. Output: `7 7`.  
   **Answer**: 7 7


2. **Solution**:
   `[[0]*2]*3` creates three references to the same inner list. Modifying `x[0][0]` affects all rows. Output: `[[1, 0], [1, 0], [1, 0]]`.  
   **Answer**: [[1, 0], [1, 0], [1, 0]]


3. **Solution**:
   `==` checks reference equality. `new String` creates distinct objects. Output: `false`.  
   **Answer**: false


4. **Solution**:
   Lambda captures `x` by reference. `f()` increments `x` to `15`, returns `15`. `x` is also `15`. Output: `15 15`.  
   **Answer**: 15 15


5. **Solution**:
   Default list `x` is shared across calls. First `f()`: `x = [1]`. Second `f()`: `x = [1, 1]`. Output: `[1] [1, 1]`.  
   **Answer**: [1] [1, 1]


6. **Solution**:
   `p` is a void pointer to `x`. Cast to `int*` and dereference gives `5`. Output: `5`.  
   **Answer**: 5


7. **Solution**:
   Integer caching for `-128` to `127` reuses objects. `a` and `b` reference the same object. Output: `true`.  
   **Answer**: true


8. **Solution**:
   `copy()` creates a shallow copy. `y[1]` references the same list as `x[1]`. Appending `3` modifies `x[1]`. Output: `[1, 3]`.  
   **Answer**: [1, 3]


9. **Solution**:
   `*(p + 1) = arr[1] = 2`, `*(p + 2) = arr[2] = 3`. `2 * 3 = 6`. Output: `6`.  
   **Answer**: 6


10. **Solution**:
    Union shares memory. `x = 258` (binary `00000001 00000010`). `c` reads first byte (`00000010` = 2). Output: `2`.  
    **Answer**: 2


11. **Solution**:
    `reduce` applies `+` with initial value `0`: `((0 + 1) + 2) + 3 = 6`. Output: `6`.  
    **Answer**: 6


12. **Solution**:
    Exception is caught, prints `Caught`. `finally` always executes. Output: `Caught Finally`.  
    **Answer**: Caught Finally


13. **Solution**:
    `transform` squares each element. `v = [1, 4, 9]`. `v[1] = 4`. Output: `4`.  
    **Answer**: 4


14. **Solution**:
    `iter(x)` creates an iterator. First `next(y)` returns `1`. Second `next(y)` returns `2`. Output: `2`.  
    **Answer**: 2


15. **Solution**:
    Undefined behavior due to multiple modifications of `x` without sequence point. Possible: `x = 7`, `y = 12` (5 + 7). Output varies, assume common compiler: `7 12`.  
    **Answer**: 7 12 (compiler-dependent)


16. **Solution**:
    `replaceAll` increments each element. `list = [2, 3, 4]`. Output: `[2, 3, 4]`.  
    **Answer**: [2, 3, 4]


17. **Solution**:
    `deepcopy` creates independent copies. Modifying `y` doesn’t affect `x`. Output: `[[1], [2]]`.  
    **Answer**: [[1], [2]]


18. **Solution**:
    Lambda captures `x` by reference. `f(3)` adds `3` to `x = 5`, returns `x = 8`. Output: `8`.  
    **Answer**: 8


19. **Solution**:
    `s.x = 10`, `s.c = 'A'`. Output: `10 A`.  
    **Answer**: 10 A


20. **Solution**:
    `filter` selects odd numbers: `[1, 3]`. Output: `[1, 3]`.  
    **Answer**: [1, 3]


## Data Structures (21–40)

21. **Solution**:
    Traverse from root to nodes, comparing values: O(h), where h is height (O(log n) if balanced).  
    **Answer**: O(log n) (balanced)


22. **Solution**:
    Tree structure: `10 -> 15 -> 20`. `root.right.right.val = 20`. Output: `20`.  
    **Answer**: 20


23. **Solution**:
    Heapify from bottom-up: O(n).  
    **Answer**: O(n)


24. **Solution**:
    DFS visits all vertices and edges: O(V + E).  
    **Answer**: O(V + E)


25. **Solution**:
    `defaultdict` creates empty list for new keys. `d[1] = [2, 3]`. Output: `defaultdict(<class 'list'>, {1: [2, 3]})`.  
    **Answer**: defaultdict(<class 'list'>, {1: [2, 3]})


26. **Solution**:
    BFS explores all vertices and edges: O(V + E).  
    **Answer**: O(V + E)


27. **Solution**:
    Traverse characters: O(k).  
    **Answer**: O(k)


28. **Solution**:
    Linked list: `1 -> 2 -> 3`. `head.next.next.val = 3`. Output: `3`.  
    **Answer**: 3


29. **Solution**:
    Sort edges O(E log E), union-find O(E α(V)) ≈ O(E log V). Total: O(E log V).  
    **Answer**: O(E log V)


30. **Solution**:
    Traverse height of tree: O(log n).  
    **Answer**: O(log n)


31. **Solution**:
    Min-heap: `[1, 2, 3]`. `heappop` removes smallest: `1`. Output: `1`.  
    **Answer**: 1


32. **Solution**:
    Rebalance after deletion: O(log n).  
    **Answer**: O(log n)


33. **Solution**:
    Relax edges V-1 times: O(V * E).  
    **Answer**: O(V * E)


34. **Solution**:
    BFS visits all nodes in graph: `1, 2, 3, 4`. `len(visited) = 4`. Output: `4`.  
    **Answer**: 4


35. **Solution**:
    Adjacency list: O(V + E).  
    **Answer**: O(V + E)


36. **Solution**:
    Traverse height: O(log_m n).  
    **Answer**: O(log n)


37. **Solution**:
    Sort by first element, then second: `[(1, 'a'), (1, 'c'), (2, 'b')]`. Output: `[(1, 'a'), (1, 'c'), (2, 'b')]`.  
    **Answer**: [(1, 'a'), (1, 'c'), (2, 'b')]


38. **Solution**:
    Two DFS passes and transpose: O(V + E).  
    **Answer**: O(V + E)


39. **Solution**:
    Traverse path matching substring: O(m), where m is substring length.  
    **Answer**: O(m)


40. **Solution**:
    `move_to_end(1)` moves key `1` to end. Keys: `[2, 1]`. Output: `[2, 1]`.  
    **Answer**: [2, 1]


## Algorithms (41–60)

41. **Solution**:
    DP table of size n × W: O(n * W).  
    **Answer**: O(n * W)


42. **Solution**:
    LCS of `"ABC"` and `"AC"` is `"AC"`. Length: `2`. Output: `2`.  
    **Answer**: 2


43. **Solution**:
    DP table for all possible splits: O(n³).  
    **Answer**: O(n³)


44. **Solution**:
    Sliding window maximum using multiset. Max of `[3,1], [1,4], [4,1], [1,5]` is `4`. Output: `4`.  
    **Answer**: 4


45. **Solution**:
    Three nested loops: O(V³).  
    **Answer**: O(V³)


46. **Solution**:
    Kadane’s algorithm finds max subarray sum: `[4, -1, 2, 1] = 6`. Output: `6`.  
    **Answer**: 6


47. **Solution**:
    Binary search to partition arrays: O(log n).  
    **Answer**: O(log n)


48. **Solution**:
    LPS for `"AABAAC"`: `[0, 1, 0, 1, 2, 0]`. `lps[5] = 0`. Output: `0`.  
    **Answer**: 0


49. **Solution**:
    Depends on heuristic, typically O(b^d) where b is branching factor, d is depth.  
    **Answer**: O(b^d)


50. **Solution**:
    Edit distance from `"cat"` to `"cut"` is 1 (replace `a` with `u`). Output: `1`.  
    **Answer**: 1


51. **Solution**:
    DP table for all substrings: O(n²).  
    **Answer**: O(n²)


52. **Solution**:
    DP computes number of paths in n×n grid: `dp[5][5] = 252` (binomial coefficient). Output: `252`.  
    **Answer**: 252


53. **Solution**:
    Rolling hash and pattern storage: O(1) extra space.  
    **Answer**: O(1)


54. **Solution**:
    Max profit by buying at `1`, selling at `6`: `6 - 1 = 5`. Output: `5`.  
    **Answer**: 5


55. **Solution**:
    Sort points O(n log n), scan O(n). Total: O(n log n).  
    **Answer**: O(n log n)


56. **Solution**:
    Catalan number for `n = 4`: `dp[4] = 14` (number of BSTs). Output: `14`.  
    **Answer**: 14


57. **Solution**:
    Maximum flow approach: O(n³).  
    **Answer**: O(n³)


58. **Solution**:
    Inversions in `[3, 1, 2]`: `(3, 1), (3, 2)`. Count: `2`. Output: `2`.  
    **Answer**: 2


59. **Solution**:
    Binary search on partitions: O(log(min(m, n))).  
    **Answer**: O(log(min(m, n)))


60. **Solution**:
    Number of ways to sum to `n` with positive integers: `dp[3] = 4` (1+1+1, 1+2, 2+1, 3). Output: `4`.  
    **Answer**: 4


## Database Basics (61–70)

61. **Solution**:
    Joins `employees` and `departments`, groups by `department_name`, computes average `salary`, filters departments with >5 employees, sorts by average salary descending.  
    **Answer**: Department names and average salaries for departments with >5 employees, sorted high to low


62. **Solution**:
    Counts orders per customer, including customers with zero orders.  
    **Answer**: Customer names and their order counts


63. **Solution**:
    Retrieves `product_name` and `price` for products priced above their category’s average.  
    **Answer**: Products above category average price


64. **Solution**:
    Automatically reduces `stock` in `products` by `quantity` after an order is inserted.  
    **Answer**: Updates product stock on order insertion


65. **Solution**:
    Retrieves names of employees with salaries above the average salary of their direct reports.  
    **Answer**: Employees earning above their team’s average


66. **Solution**:
    Provides query execution plan, showing how the database processes the query.  
    **Answer**: Shows query plan


67. **Solution**:
    Lists maximum `price` per `category`, plus overall maximum `price` labeled as `'Total'`.  
    **Answer**: Category max prices and overall max price


68. **Solution**:
    Adds a unique constraint to `email` column, preventing duplicate emails.  
    **Answer**: Enforces unique emails


69. **Solution**:
    Retrieves `name` of students who have at least one course with grade `'A'`.  
    **Answer**: Students with A-grade courses


70. **Solution**:
    Creates a virtual table showing `name` and `salary` for employees with `salary > 100000`.  
    **Answer**: Creates high-salary view


## Computer Networks (71–80)

71. **Solution**:
    Provides reliable data transfer, flow control, and error correction.  
    **Answer**: Reliable data transfer


72. **Solution**:
    Provides encryption and authentication for IP packets.  
    **Answer**: Secures IP communication


73. **Solution**:
    TCP: single stream, reliable; SCTP: multi-stream, supports multi-homing.  
    **Answer**: TCP: single stream, SCTP: multi-stream


74. **Solution**:
    Dynamically assigns IP addresses to devices on a network.  
    **Answer**: IP address assignment


75. **Solution**:
    Limits packet lifetime to prevent infinite loops (decremented per hop).  
    **Answer**: Prevents routing loops


76. **Solution**:
    Stateful: tracks connection states; Stateless: filters packets based on rules.  
    **Answer**: Stateful: connection-aware, Stateless: rule-based


77. **Solution**:
    Resets a connection due to errors or invalid segments.  
    **Answer**: Connection reset


78. **Solution**:
    Simple Network Management Protocol monitors and manages network devices.  
    **Answer**: Network monitoring


79. **Solution**:
    Throughput = Window Size / RTT = (64 * 1024 * 8) / (10 / 1000) = 51.2 Mbps.  
    **Answer**: 51.2 Mbps


80. **Solution**:
    Adds identifiers to frames to separate traffic on virtual LANs.  
    **Answer**: Separates VLAN traffic


## Operating Systems (81–90)

81. **Solution**:
    Spinlock: busy-waits in a loop; Semaphore: blocks threads, supports counting.  
    **Answer**: Spinlock: busy-wait, Semaphore: blocking


82. **Solution**:
    Caches recent virtual-to-physical address translations to speed up access.  
    **Answer**: Speeds address translation


83. **Solution**:
    Prevents deadlock by ensuring safe resource allocation.  
    **Answer**: Deadlock avoidance


84. **Solution**:
    User-level: managed by application, no kernel involvement; Kernel-level: OS-managed, supports parallelism.  
    **Answer**: User-level: app-managed, Kernel-level: OS-managed


85. **Solution**:
    Delays copying shared memory pages until a write occurs, saving resources.  
    **Answer**: Optimizes memory usage


86. **Solution**:
    Maps physical pages to virtual pages, reducing memory overhead.  
    **Answer**: Efficient page mapping


87. **Solution**:
    Hard: strict deadlines, failure is critical; Soft: deadlines important but not critical.  
    **Answer**: Hard: critical, Soft: non-critical


88. **Solution**:
    Ensures mutual exclusion and provides condition variables for synchronization.  
    **Answer**: Synchronization construct


89. **Solution**:
    Optimizes disk access by reordering I/O requests.  
    **Answer**: Optimizes disk I/O


90. **Solution**:
    Demand paging: loads pages on demand; Prepaging: loads pages in advance to reduce faults.  
    **Answer**: Demand: on-demand, Prepaging: anticipatory


## AI/ML Foundations (91–100)

91. **Solution**:
    L1: adds absolute weights (sparsity); L2: adds squared weights (smoothness).  
    **Answer**: L1: sparsity, L2: smoothness


92. **Solution**:
    Halts training when validation performance stops improving to prevent overfitting.  
    **Answer**: Prevents overfitting


93. **Solution**:
    Normalizes layer inputs to stabilize and accelerate training.  
    **Answer**: Stabilizes training


94. **Solution**:
    Precision: TP/(TP+FP) (accuracy of positive predictions); Recall: TP/(TP+FN) (coverage of actual positives).  
    **Answer**: Precision: accuracy, Recall: coverage


95. **Solution**:
    Randomly deactivates neurons during training to prevent overfitting.  
    **Answer**: Reduces overfitting


96. **Solution**:
    CNN: processes spatial data (e.g., images); RNN: processes sequential data (e.g., time series).  
    **Answer**: CNN: spatial, RNN: sequential


97. **Solution**:
    Weights input elements based on relevance, improving context understanding.  
    **Answer**: Focuses on relevant inputs


98. **Solution**:
    Harmonic mean of precision and recall, balances both metrics.  
    **Answer**: Balances precision and recall


99. **Solution**:
    Generative: models joint probability P(x,y); Discriminative: models conditional P(y|x).  
    **Answer**: Generative: joint, Discriminative: conditional


100. **Solution**:
     Uses pre-trained models to improve performance on new tasks with less data.  
     **Answer**: Leverages pre-trained models
