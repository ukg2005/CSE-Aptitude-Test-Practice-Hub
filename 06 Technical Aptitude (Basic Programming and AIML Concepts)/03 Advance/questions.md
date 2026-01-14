# 100 Technical Aptitude Practice Questions (Advanced Level)

## Programming Fundamentals (1–20)

1. **Question**: What is the output of this C code: `int x = 5; int *p = &x; *p += 2; printf("%d %d", x, *p);`?  

2. **Question**: In Python, what is the output of: `x = [[0]*2]*3; x[0][0] = 1; print(x)`?  

3. **Question**: In Java, what is the output of: `String s1 = new String("test"); String s2 = new String("test"); System.out.println(s1 == s2);`?  

4. **Question**: In C++, what is the output of: `int x = 10; auto f = [&x]() { x += 5; return x; }; cout << f() << " " << x;`?  

5. **Question**: In Python, what is the output of: `def f(x=[]): x.append(1); return x; print(f(), f())`?  

6. **Question**: In C, what is the output of: `int x = 5; void *p = &x; printf("%d", *(int*)p);`?  

7. **Question**: In Java, what is the output of: `Integer a = 127; Integer b = 127; System.out.println(a == b);`?  

8. **Question**: In Python, what is the output of: `x = {1: [1], 2: [2]}; y = x.copy(); y[1].append(3); print(x[1])`?  

9. **Question**: In C++, what is the output of: `int arr[] = {1, 2, 3}; int *p = arr; cout << *(p + 1) * *(p + 2);`?  

10. **Question**: In C, what is the output of: `union U { int x; char c; } u; u.x = 258; printf("%d", u.c);`?  

11. **Question**: In Python, what is the output of: `from functools import reduce; print(reduce(lambda x, y: x + y, [1, 2, 3], 0))`?  

12. **Question**: In Java, what is the output of: `try { throw new Exception("Error"); } catch (Exception e) { System.out.println("Caught"); } finally { System.out.println("Finally"); }`?  

13. **Question**: In C++, what is the output of: `vector<int> v = {1, 2, 3}; transform(v.begin(), v.end(), v.begin(), [](int x) { return x * x; }); cout << v[1];`?  

14. **Question**: In Python, what is the output of: `x = [1, 2, 3]; y = iter(x); next(y); print(next(y))`?  

15. **Question**: In C, what is the output of: `int x = 5; int y = x++ + ++x; printf("%d %d", x, y);`?  

16. **Question**: In Java, what is the output of: `List<Integer> list = Arrays.asList(1, 2, 3); list.replaceAll(x -> x + 1); System.out.println(list);`?  

17. **Question**: In Python, what is the output of: `import copy; x = [[1], [2]]; y = copy.deepcopy(x); y[0].append(3); print(x)`?  

18. **Question**: In C++, what is the output of: `int x = 5; function<int(int)> f = [&](int a) { x += a; return x; }; cout << f(3);`?  

19. **Question**: In C, what is the output of: `struct S { int x; char c; } s = {10, 'A'}; printf("%d %c", s.x, s.c);`?  

20. **Question**: In Python, what is the output of: `x = [1, 2, 3]; print(list(filter(lambda x: x % 2 == 1, x)))`?  

## Data Structures (21–40)

21. **Question**: What is the time complexity of finding the lowest common ancestor (LCA) in a binary search tree with n nodes?  

22. **Question**: In Python, what is the output of this AVL tree insertion (simplified): `class Node: def __init__(self, val): self.val = val; self.left = self.right = None; root = Node(10); root.left = Node(5); root.right = Node(15); root.right.right = Node(20); print(root.right.right.val)`?  

23. **Question**: What is the time complexity of building a binary heap from an array of n elements?  

24. **Question**: In a graph with V vertices and E edges, what is the time complexity of detecting a cycle using DFS?  

25. **Question**: In Python, what is the output of: `from collections import defaultdict; d = defaultdict(list); d[1].append(2); d[1].append(3); print(d)`?  

26. **Question**: What is the time complexity of finding the shortest path in an unweighted graph using BFS?  

27. **Question**: In a trie with n words of average length k, what is the time complexity to search for a word?  

28. **Question**: In Python, what is the output of: `class Node: def __init__(self, val): self.val = val; self.next = None; head = Node(1); head.next = Node(2); head.next.next = Node(3); print(head.next.next.val)`?  

29. **Question**: What is the time complexity of Kruskal’s algorithm for minimum spanning tree with V vertices and E edges?  

30. **Question**: In a segment tree for range sum queries with n elements, what is the time complexity of a query?  

31. **Question**: In Python, what is the output of: `from heapq import heappush, heappop; h = []; heappush(h, 3); heappush(h, 1); heappush(h, 2); print(heappop(h))`?  

32. **Question**: What is the time complexity of deleting a node from a red-black tree with n nodes?  

33. **Question**: In a weighted graph, what is the time complexity of Bellman-Ford algorithm for single-source shortest paths?  

34. **Question**: In Python, what is the output of: `from collections import deque; g = {1: [2, 3], 2: [4], 3: [4], 4: []}; q = deque([1]); visited = {1}; while q: n = q.popleft(); for nei in g[n]: if nei not in visited: visited.add(nei); q.append(nei); print(len(visited))`?  

35. **Question**: What is the space complexity of storing a sparse graph with V vertices and E edges?  

36. **Question**: In a B-tree of order m with n keys, what is the time complexity of searching a key?  

37. **Question**: In Python, what is the output of: `x = [(1, 'a'), (2, 'b'), (1, 'c')]; x.sort(); print(x)`?  

38. **Question**: What is the time complexity of finding strongly connected components using Kosaraju’s algorithm?  

39. **Question**: In a suffix tree for a string of length n, what is the time complexity to check if a substring exists?  

40. **Question**: In Python, what is the output of: `from collections import OrderedDict; d = OrderedDict([(1, 'a'), (2, 'b')]); d.move_to_end(1); print(list(d.keys()))`?  

## Algorithms (41–60)

41. **Question**: What is the time complexity of the knapsack problem (0/1) using dynamic programming for n items and capacity W?  

42. **Question**: In Python, what is the output of this longest common subsequence: `def lcs(s1, s2): m, n = len(s1), len(s2); dp = [[0]*(n+1) for _ in range(m+1)]; for i in range(1, m+1): for j in range(1, n+1): if s1[i-1] == s2[j-1]: dp[i][j] = dp[i-1][j-1] + 1; else: dp[i][j] = max(dp[i-1][j], dp[i][j-1]); return dp[m][n]; print(lcs("ABC", "AC"))`?  

43. **Question**: What is the time complexity of matrix chain multiplication for n matrices using dynamic programming?  

44. **Question**: In C++, what is the output of: `vector<int> v = {3, 1, 4, 1, 5}; int k = 2; multiset<int> s(v.begin(), v.begin()+k); int ans = *s.rbegin(); for(int i = k; i < v.size(); i++) { s.erase(s.find(v[i-k])); s.insert(v[i]); ans = max(ans, *s.rbegin()); } cout << ans;`?  

45. **Question**: What is the time complexity of Floyd-Warshall algorithm for all-pairs shortest paths in a graph with V vertices?  

46. **Question**: In Python, what is the output of: `def kadane(arr): max_so_far = max_ending_here = arr[0]; for x in arr[1:]: max_ending_here = max(x, max_ending_here + x); max_so_far = max(max_so_far, max_ending_here); return max_so_far; print(kadane([-2, 1, -3, 4, -1, 2, 1]))`?  

47. **Question**: What is the time complexity of finding the median of two sorted arrays of size n each?  

48. **Question**: In C, what is the output of this KMP preprocessing: `void computeLPS(char *pat, int m, int *lps) { int len = 0, i = 1; lps[0] = 0; while(i < m) { if(pat[i] == pat[len]) { len++; lps[i++] = len; } else if(len > 0) len = lps[len-1]; else lps[i++] = 0; } } int lps[6]; computeLPS("AABAAC", 6, lps); printf("%d", lps[5]);`?  

49. **Question**: What is the time complexity of the A* search algorithm in a graph?  

50. **Question**: In Python, what is the output of: `def edit_distance(s1, s2): m, n = len(s1), len(s2); dp = [[0]*(n+1) for _ in range(m+1)]; for i in range(m+1): dp[i][0] = i; for j in range(n+1): dp[0][j] = j; for i in range(1, m+1): for j in range(1, n+1): if s1[i-1] == s2[j-1]: dp[i][j] = dp[i-1][j-1]; else: dp[i][j] = min(dp[i-1][j], dp[i][j-1], dp[i-1][j-1]) + 1; return dp[m][n]; print(edit_distance("cat", "cut"))`?  

51. **Question**: What is the time complexity of finding the longest palindromic substring using dynamic programming?  

52. **Question**: In C++, what is the output of: `int n = 5; vector<vector<int>> dp(n+1, vector<int>(n+1)); for(int i = 0; i <= n; i++) dp[i][0] = dp[0][i] = 1; for(int i = 1; i <= n; i++) for(int j = 1; j <= n; j++) dp[i][j] = dp[i-1][j] + dp[i][j-1]; cout << dp[n][n];`?  

53. **Question**: What is the space complexity of the Rabin-Karp string matching algorithm?  

54. **Question**: In Python, what is the output of: `def max_profit(prices): n = len(prices); if n < 2: return 0; dp = [0]*n; min_price = prices[0]; for i in range(1, n): min_price = min(min_price, prices[i]); dp[i] = max(dp[i-1], prices[i] - min_price); return dp[n-1]; print(max_profit([7, 1, 5, 3, 6, 4]))`?  

55. **Question**: What is the time complexity of computing the convex hull of n points using Graham’s scan?  

56. **Question**: In C, what is the output of: `int n = 4; int dp[5]; dp[0] = 1; for(int i = 1; i <= n; i++) { dp[i] = 0; for(int j = 0; j < i; j++) dp[i] += dp[j] * dp[i-j-1]; } printf("%d", dp[n]);`?  

57. **Question**: What is the time complexity of the Hungarian algorithm for bipartite matching with n vertices?  

58. **Question**: In Python, what is the output of: `def count_inversions(arr): def merge_and_count(l, r): inv = 0; res = []; i = j = 0; while i < len(l) and j < len(r): if l[i] <= r[j]: res.append(l[i]); i += 1; else: res.append(r[j]); inv += len(l)-i; j += 1; res.extend(l[i:]); res.extend(r[j:]); return res, inv; def sort_and_count(arr): if len(arr) <= 1: return arr, 0; mid = len(arr)//2; l, inv_l = sort_and_count(arr[:mid]); r, inv_r = sort_and_count(arr[mid:]); merged, inv_m = merge_and_count(l, r); return merged, inv_l + inv_r + inv_m; _, inv = sort_and_count([3, 1, 2]); print(inv)`?  

59. **Question**: What is the time complexity of finding the k-th smallest element in two sorted arrays of sizes m and n?  

60. **Question**: In C++, what is the output of: `int n = 3; vector<int> dp(n+1); dp[0] = 1; for(int i = 1; i <= n; i++) for(int j = 1; j <= i; j++) dp[i] += dp[i-j]; cout << dp[n];`?  

## Database Basics (61–70)

61. **Question**: What is the result of this SQL query: `SELECT d.department_name, AVG(e.salary) FROM employees e JOIN departments d ON e.department_id = d.id GROUP BY d.department_name HAVING COUNT(e.id) > 5 ORDER BY AVG(e.salary) DESC;`?  

62. **Question**: What does `SELECT c.customer_name, COUNT(o.order_id) FROM customers c LEFT JOIN orders o ON c.id = o.customer_id GROUP BY c.customer_name;` do?  

63. **Question**: What is the output of: `SELECT product_name, price FROM products WHERE price > (SELECT AVG(price) FROM products WHERE category = products.category);`?  

64. **Question**: What does `CREATE TRIGGER update_stock AFTER INSERT ON orders FOR EACH ROW UPDATE products SET stock = stock - NEW.quantity WHERE id = NEW.product_id;` do?  

65. **Question**: What is the result of: `SELECT e1.name FROM employees e1 WHERE e1.salary > (SELECT AVG(e2.salary) FROM employees e2 WHERE e2.manager_id = e1.id);`?  

66. **Question**: What does `EXPLAIN SELECT * FROM orders WHERE customer_id = 100;` do?  

67. **Question**: What is the output of: `SELECT category, MAX(price) FROM products GROUP BY category UNION SELECT 'Total', MAX(price) FROM products;`?  

68. **Question**: What does `ALTER TABLE employees ADD CONSTRAINT unique_email UNIQUE (email);` do?  

69. **Question**: What is the result of: `SELECT name FROM students s WHERE EXISTS (SELECT 1 FROM courses c WHERE c.student_id = s.id AND c.grade = 'A');`?  

70. **Question**: What does `CREATE VIEW high_salary AS SELECT name, salary FROM employees WHERE salary > 100000;` do?  

## Computer Networks (71–80)

71. **Question**: What is the purpose of the Transport layer in the OSI model?  

72. **Question**: What is the role of IPSec in network security?  

73. **Question**: What is the difference between TCP and SCTP?  

74. **Question**: What is the purpose of the DHCP protocol?  

75. **Question**: What is the role of the TTL field in an IP header?  

76. **Question**: What is the difference between stateful and stateless firewalls?  

77. **Question**: What is the purpose of the RST flag in TCP?  

78. **Question**: What is the role of SNMP in network management?  

79. **Question**: What is the maximum throughput of a network with 100 Mbps bandwidth and 10 ms RTT, assuming TCP with window size 64 KB?  

80. **Question**: What is the purpose of VLAN tagging in Ethernet networks?  

## Operating Systems (81–90)

81. **Question**: What is the difference between spinlock and semaphore in an OS?  

82. **Question**: What is the role of the TLB (Translation Lookaside Buffer) in virtual memory?  

83. **Question**: What is the Banker’s algorithm used for in an OS?  

84. **Question**: What is the difference between user-level and kernel-level threads?  

85. **Question**: What is the purpose of copy-on-write in memory management?  

86. **Question**: What is the role of the inverted page table in an OS?  

87. **Question**: What is the difference between hard and soft real-time systems?  

88. **Question**: What is the purpose of the monitor in process synchronization?  

89. **Question**: What is the role of the I/O scheduler in an OS?  

90. **Question**: What is the difference between demand paging and prepaging?  

## AI/ML Foundations (91–100)

91. **Question**: What is the difference between L1 and L2 regularization in ML?  

92. **Question**: What is the purpose of early stopping in neural network training?  

93. **Question**: What is the role of batch normalization in deep learning?  

94. **Question**: What is the difference between precision and recall in ML evaluation?  

95. **Question**: What is the purpose of dropout in neural networks?  

96. **Question**: What is the difference between CNN and RNN architectures?  

97. **Question**: What is the role of the attention mechanism in transformers?  

98. **Question**: What is the purpose of the F1 score in ML evaluation?  

99. **Question**: What is the difference between generative and discriminative models in ML?  

100. **Question**: What is the purpose of transfer learning in deep learning?
