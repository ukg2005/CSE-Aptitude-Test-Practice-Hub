# 100 Technical Aptitude Practice Questions (Intermediate Level)

## Programming Fundamentals (1–20)

1. **Question**: What is the output of this C code: `int x = 5; printf("%d %d", x++, ++x);`?  

2. **Question**: In Python, what is the output of: `x = [1, 2, 3]; y = x; y[0] = 4; print(x)`?  

3. **Question**: In Java, what is the output of: `String s = "hello"; s = s.concat(" world"); System.out.println(s);`?  

4. **Question**: In C++, what is the output of: `int x = 10; cout << (x > 5 ? x : 5);`?  

5. **Question**: In Python, what is the output of: `def f(x): x += 1; x = 5; f(x); print(x)`?  

6. **Question**: In C, what is the output of: `int x = 10; printf("%d", x << 2);`?  

7. **Question**: In Java, what is the output of: `int[] arr = {1, 2, 3}; System.out.println(arr[arr.length - 1]);`?  

8. **Question**: In Python, what is the output of: `x = {1: 'a', 2: 'b'}; x.update({2: 'c'}); print(x)`?  

9. **Question**: In C++, what is the output of: `int x = 5; for(int i = 0; i < 3; i++) x *= 2; cout << x;`?  

10. **Question**: In C, what is the output of: `int a = 7, b = 3; printf("%d", a ^ b);`?  

11. **Question**: In Python, what is the output of: `x = [1, 2, 3]; print(x[1:3])`?  

12. **Question**: In Java, what is the output of: `int x = 15; System.out.println(x & (x - 1));`?  

13. **Question**: In C++, what is the output of: `string s = "abc"; reverse(s.begin(), s.end()); cout << s;`?  

14. **Question**: In Python, what is the output of: `x = lambda a: a * 2; print(x(3))`?  

15. **Question**: In C, what is the output of: `int x = 5; printf("%d", ~x);`?  

16. **Question**: In Java, what is the output of: `int x = 8; System.out.println(x >> 1);`?  

17. **Question**: In Python, what is the output of: `x = [1, 2]; y = x.copy(); y[0] = 3; print(x)`?  

18. **Question**: In C++, what is the output of: `int x = 3; cout << (x << 1) + (x >> 1);`?  

19. **Question**: In C, what is the output of: `int arr[3] = {1, 2, 3}; printf("%d", *(arr + 1));`?  

20. **Question**: In Python, what is the output of: `x = [1, 2, 3]; print(list(map(lambda x: x**2, x)))`?  

## Data Structures (21–40)

21. **Question**: What is the time complexity of inserting a node at the end of a singly linked list with n nodes?  

22. **Question**: In Python, what is the output of this stack operation: `s = []; s.append(1); s.append(2); s.append(3); s.pop(); s.pop(); print(s)`?  

23. **Question**: In a doubly linked list, what is the time complexity to delete a node given its pointer?  

24. **Question**: In a queue, after enqueue(1, 2, 3), dequeue(), enqueue(4), dequeue(), what is the front element?  

25. **Question**: What is the time complexity of searching in an unbalanced binary search tree with n nodes?  

26. **Question**: In Python, what is the output of: `from collections import deque; q = deque([1, 2]); q.append(3); q.popleft(); print(q)`?  

27. **Question**: What is the time complexity of inserting an element in a min-heap with n elements?  

28. **Question**: In a binary tree, what is the time complexity of finding the height?  

29. **Question**: In Python, what is the output of: `d = {'a': 1, 'b': 2}; d.pop('a'); print(d)`?  

30. **Question**: What is the time complexity of deleting the root of a max-heap with n elements?  

31. **Question**: In a circular linked list, what is the time complexity to insert a node after a given node?  

32. **Question**: In Python, what is the output of: `s = {1, 2, 3}; s.discard(2); print(s)`?  

33. **Question**: In a binary search tree, what is the time complexity to find the minimum element?  

34. **Question**: What is the space complexity of a depth-first search (DFS) on a binary tree with n nodes?  

35. **Question**: In Python, what is the output of: `x = [[1, 2], [3, 4]]; x[0].append(5); print(x)`?  

36. **Question**: What is the time complexity of level-order traversal (BFS) of a binary tree with n nodes?  

37. **Question**: In a hash table with chaining, what is the average time complexity for search with n elements and m buckets?  

38. **Question**: In Python, what is the output of: `from collections import Counter; c = Counter([1, 2, 2, 3]); print(c[2])`?  

39. **Question**: What is the time complexity to check if a binary tree is balanced?  

40. **Question**: In a stack, after push(1, 2, 3), pop(), push(4), pop(), what is the top element?  

## Algorithms (41–60)

41. **Question**: What is the time complexity of merge sort for n elements?  

42. **Question**: In Python, what is the output of this binary search: `def bs(arr, t): l, r = 0, len(arr)-1; while l <= r: m = (l+r)//2; if arr[m] == t: return m; elif arr[m] < t: l = m+1; else: r = m-1; return -1; print(bs([1, 2, 3, 4], 3))`?  

43. **Question**: What is the space complexity of quicksort?  

44. **Question**: In C, what is the output of this GCD code: `int gcd(int a, int b) { if(b == 0) return a; return gcd(b, a % b); } printf("%d", gcd(48, 18));`?  

45. **Question**: What is the time complexity of finding all pairs in an array of n elements that sum to a given value?  

46. **Question**: In Python, what is the output of: `x = [4, 2, 5, 1]; x.sort(); print(x)`?  

47. **Question**: What is the time complexity of Dijkstra’s algorithm using a priority queue for a graph with V vertices and E edges?  

48. **Question**: In C++, what is the output of: `vector<int> v = {1, 2, 3}; rotate(v.begin(), v.begin()+1, v.end()); cout << v[0];`?  

49. **Question**: What is the time complexity of insertion sort for n elements?  

50. **Question**: In Python, what is the output of: `x = [1, 2, 3, 4]; print([i for i in x if i % 2 == 0])`?  

51. **Question**: What is the time complexity of checking if a string is a palindrome?  

52. **Question**: In C, what is the output of this Fibonacci code: `int fib(int n) { if(n <= 1) return n; return fib(n-1) + fib(n-2); } printf("%d", fib(5));`?  

53. **Question**: What is the space complexity of merge sort?  

54. **Question**: In Python, what is the output of: `x = "hello"; print(''.join(reversed(x)))`?  

55. **Question**: What is the time complexity of finding the longest common prefix of n strings of length m?  

56. **Question**: In C++, what is the output of: `int arr[] = {1, 2, 3}; int *p = arr; cout << *(p + 2);`?  

57. **Question**: What is the time complexity of counting sort for n elements with range k?  

58. **Question**: In Python, what is the output of: `x = [1, 2, 2, 3]; print(list(set(x)))`?  

59. **Question**: What is the time complexity of detecting a cycle in a linked list?  

60. **Question**: In C, what is the output of: `int arr[] = {3, 1, 4}; qsort(arr, 3, sizeof(int), [](const void* a, const void* b){return *(int*)a - *(int*)b;}); printf("%d", arr[0]);`?  

## Database Basics (61–70)

61. **Question**: What is the result of this SQL query: `SELECT name, salary FROM employees WHERE department = 'IT' ORDER BY salary DESC;`?  

62. **Question**: What does `SELECT * FROM orders INNER JOIN customers ON orders.customer_id = customers.id;` do?  

63. **Question**: What is the output of: `SELECT department, COUNT(*) FROM employees GROUP BY department;`?  

64. **Question**: What does `FOREIGN KEY` constraint ensure in SQL?  

65. **Question**: What is the result of: `SELECT product_name FROM products WHERE price BETWEEN 50 AND 100;`?  

66. **Question**: What does `SELECT DISTINCT city FROM customers;` do?  

67. **Question**: What is the output of: `SELECT name FROM students WHERE marks > (SELECT AVG(marks) FROM students);`?  

68. **Question**: What does `ALTER TABLE employees ADD COLUMN email VARCHAR(100);` do?  

69. **Question**: What is the result of: `SELECT order_id, customer_name FROM orders LEFT JOIN customers ON orders.customer_id = customers.id;`?  

70. **Question**: What does `CREATE INDEX idx_name ON employees(name);` do?  

## Computer Networks (71–80)

71. **Question**: What is the purpose of the OSI model?  

72. **Question**: Which layer of the OSI model handles routing of packets?  

73. **Question**: What is the port number used by HTTPS?  

74. **Question**: What is the purpose of NAT (Network Address Translation)?  

75. **Question**: What is the difference between a hub and a switch?  

76. **Question**: What is the role of the MAC address?  

77. **Question**: What does the TCP three-way handshake involve?  

78. **Question**: What is the purpose of ICMP?  

79. **Question**: What is the maximum number of hosts in a subnet with mask 255.255.255.240?  

80. **Question**: What is the role of BGP in networking?  

## Operating Systems (81–90)

81. **Question**: What is the difference between preemptive and non-preemptive scheduling?  

82. **Question**: What is a semaphore in an operating system?  

83. **Question**: What is the purpose of paging in memory management?  

84. **Question**: What is the difference between a process and a thread?  

85. **Question**: What is the role of the swap space in an OS?  

86. **Question**: What is a context switch in an operating system?  

87. **Question**: What is the purpose of the LRU page replacement algorithm?  

88. **Question**: What is a race condition in an OS?  

89. **Question**: What is the role of the file allocation table (FAT) in a file system?  

90. **Question**: What is the purpose of a mutex in an OS?  

## AI/ML Foundations (91–100)

91. **Question**: What is the difference between classification and regression in ML?  

92. **Question**: What is the purpose of cross-validation in ML?  

93. **Question**: What is the bias-variance tradeoff in ML?  

94. **Question**: What is the role of the learning rate in gradient descent?  

95. **Question**: What is the purpose of regularization in ML?  

96. **Question**: What is the difference between a perceptron and a multi-layer perceptron (MLP)?  

97. **Question**: What is the purpose of the softmax function in neural networks?  

98. **Question**: What is the role of k in k-nearest neighbors (k-NN)?  

99. **Question**: What is the difference between bagging and boosting in ML?  

100. **Question**: What is the purpose of principal component analysis (PCA) in ML?
