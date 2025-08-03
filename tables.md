
| 🧩 **Pattern**         | 📘 **Problem Type**                           | 🧰 **Data Structure Used** | ⏱️ **Time** | 🧮 **Space** |
| ---------------------- | --------------------------------------------- | -------------------------- | ----------- | ------------ |
| 🔲 **Sliding Window**  | Fixed or variable subarray analysis           | ➖ Variables / Queue        | O(n)        | O(1) or O(k) |
| 👣 **Two Pointers**    | Find pairs, move in from ends                 | ➖ Indexes only             | O(n)        | O(1)         |
| ➕ **Prefix Sum**       | Subarray/range sum queries                    | 📋 Array                   | O(n)        | O(n)         |
| 🧠 **Hashing**         | Duplicates, frequency, lookup                 | 🗂️ HashMap / Set          | O(n)        | O(n)         |
| 🔍 **Binary Search**   | Search in sorted array                        | 📋 Array                   | O(log n)    | O(1)         |
| 🧠 **Greedy**          | Make best local choices to get optimal result | 📋 Array (sorted)          | O(n log n)  | O(1)         |
| 📉 **Monotonic Stack** | Next Greater Element, Stock Span problems     | 🧱 Stack                   | O(n)        | O(n)         |






| 🔢     | 🧠 Pattern / Algorithm          | ⏱️ Time Complexity        | 💾 Space Complexity | 🔍 Use Case Keywords                            |
| ------ | ------------------------------- | ------------------------- | ------------------- | ----------------------------------------------- |
| 1️⃣    | 🔄 **Sliding Window**           | `O(n)`                    | `O(1)` / `O(k)`     | 📏 Subarray, sum, average, max/min window       |
| 2️⃣    | 🎯 **Two Pointers**             | `O(n)`                    | `O(1)`              | 🎯 Sorted array, pair sum, reverse, move zeroes |
| 3️⃣    | ➕ **Prefix Sum / Difference**   | `O(n)`                    | `O(n)`              | 🧮 Range sum, subarray sum, balanced array      |
| 4️⃣    | 🧠 **Hashing (Map / Set)**      | `O(n)`                    | `O(n)`              | 🔍 Frequency, duplicates, lookup, anagrams      |
| 5️⃣    | 🔃 **Sorting**                  | `O(n log n)`              | `O(1)` to `O(n)`    | 🗂️ Order elements, intervals, greedy prep      |
| 6️⃣    | 💡 **Greedy**                   | `O(n)` or `O(n log n)`    | `O(1)`              | ⚡ Pick best option at every step, jobs, coins   |
| 7️⃣    | 🧮 **Binary Search**            | `O(log n)` / `O(log max)` | `O(1)`              | 🎯 Search position, peak element, rotation      |
| 8️⃣    | 📏 **Monotonic Stack / Queue**  | `O(n)`                    | `O(n)`              | 📊 NGE, stock span, sliding window max          |
| 9️⃣    | 🔢 **Bit Manipulation**         | `O(n)`                    | `O(1)`              | 💡 XOR, set bits, power of 2, bitmask           |
| 🔟     | 🔁 **Backtracking**             | `O(2^n)` / `O(n!)`        | `O(n)`              | 🌀 Subsets, permutations, combinations          |
| 1️⃣1️⃣ | 📈 **Kadane’s Algorithm**       | `O(n)`                    | `O(1)`              | 💥 Max subarray sum                             |
| 1️⃣2️⃣ | ⚔️ **Divide & Conquer**         | `O(n log n)`              | `O(log n)`          | 🧩 Merge sort, max subarray, binary tricks      |
| 1️⃣3️⃣ | 🚦 **Dutch National Flag Algo** | `O(n)`                    | `O(1)`              | 🎨 Sort 0s, 1s, 2s / 3-way partition            |
| 1️⃣4️⃣ | 🌀 **Fast & Slow Pointers**     | `O(n)`                    | `O(1)`              | 🔄 Cycle detection, repeated numbers            |


🎯 Quick Pattern Matching
| 🧩 Problem Says...               | 💡 Use This Pattern        |
| -------------------------------- | -------------------------- |
| "Find max/min in subarray"       | 🔄 Sliding Window          |
| "Pair with sum / diff / product" | 🎯 Two Pointers or Hashing |
| "Range sum / subarray = k"       | ➕ Prefix Sum               |
| "Frequency, duplicates, lookup"  | 🧠 HashMap / HashSet       |
| "Find position, rotation, peak"  | 🧮 Binary Search           |
| "Next Greater Element / Stock"   | 📏 Monotonic Stack         |
| "Unique subset / permutation"    | 🔁 Backtracking            |
| "Cycle / repeated value"         | 🌀 Fast & Slow Pointers    |
| "Optimal choice at every step"   | 💡 Greedy                  |
| "Sort or merge recursively"      | ⚔️ Divide & Conquer        |

📊 🔃 Sorting Algorithms – Summary Table
| 🔢 Algo        | 🔧 Type        | ⏱️ Time (Best / Avg / Worst)         | 💾 Space | 🔍 Stable | 🌟 Use Case                   |
| -------------- | -------------- | ------------------------------------ | -------- | --------- | ----------------------------- |
| 🫧 Bubble Sort | Comparison     | O(n) / O(n²) / O(n²)                 | O(1)     | ✅ Yes     | Teaching basics, small data   |
| 🪣 Selection   | Comparison     | O(n²) / O(n²) / O(n²)                | O(1)     | ❌ No      | Simple, but not efficient     |
| 🃏 Insertion   | Comparison     | O(n) / O(n²) / O(n²)                 | O(1)     | ✅ Yes     | Nearly sorted data            |
| 🌊 Merge Sort  | Divide & Conq. | O(n log n) / O(n log n) / O(n log n) | O(n)     | ✅ Yes     | Linked lists, stable sort     |
| 🔥 Quick Sort  | Divide & Conq. | O(n log n) / O(n log n) / O(n²)      | O(log n) | ❌ No      | Fastest on average            |
| 🧊 Heap Sort   | Comparison     | O(n log n) / O(n log n) / O(n log n) | O(1)     | ❌ No      | Large data, priority queues   |
| 🧺 Bucket Sort | Distribution   | O(n+k)                               | O(n+k)   | ✅ Yes     | Uniform distribution          |
| ⬆️ Counting    | Non-comparison | O(n+k)                               | O(k)     | ✅ Yes     | Integers, bounded range       |
| 🧮 Radix Sort  | Non-comparison | O(nk)                                | O(n+k)   | ✅ Yes     | Fixed-length integers/strings |
📘 Tips:
Stable sort keeps equal elements in the original order.

Use Counting/Radix/Bucket when data is in a known range and integer-based.

Merge sort is stable but needs extra space.

Quick sort is the go-to for in-place fast sorting (except in worst case).


| Algorithm                | Time Complexity  | Space      | Stable | Use When...                         |
| ------------------------ | ---------------- | ---------- | ------ | ----------------------------------- |
| 🔷 Bubble Sort           | `O(n^2)`         | `O(1)`     | ✅      | Educational, not used in practice   |
| 🔷 Selection Sort        | `O(n^2)`         | `O(1)`     | ❌      | Simple, but inefficient             |
| 🔷 Insertion Sort        | `O(n^2)`         | `O(1)`     | ✅      | Nearly sorted input                 |
| ⚡ Merge Sort             | `O(n log n)`     | `O(n)`     | ✅      | Stable, reliable divide-and-conquer |
| ⚡ Quick Sort             | `O(n log n)` avg | `O(log n)` | ❌      | Fastest in practice, but unstable   |
| ⚙️ Heap Sort             | `O(n log n)`     | `O(1)`     | ❌      | Space-efficient, not stable         |
| 🔥 TimSort (Java/Python) | `O(n log n)`     | `O(n)`     | ✅      | Built-in sort (optimized hybrid)    |



| 💬 If Problem Mentions...            | 💡 Use Sorting To...                   |
| ------------------------------------ | -------------------------------------- |
| "Intervals", "Merge", "Schedule"     | Sort by start/end time                 |
| "Kth smallest/largest"               | Sort or use QuickSelect / Heap         |
| "Custom order / Comparator"          | Write a custom sort function           |
| "Greedy choices"                     | Sort first to optimize decision-making |
| "Group / categorize / organize data" | Sort for grouping                      |
| "Need sorted array as a base"        | Preprocess with sorting                |


🧱 Data Structures Used in Bit Manipulation Problems

| 📦 Data Structure                         | 📌 Purpose / Why It's Used                                       |
| ----------------------------------------- | ---------------------------------------------------------------- |
| 🔢 **Primitive Integers (`int`, `long`)** | Directly store and manipulate bits                               |
| 📋 **Array**                              | Count set bits per position, store results of multiple XORs      |
| 🧠 **HashMap / HashSet**                  | Handle duplicates or group numbers with same bit patterns        |
| 🔢 **Bitmask (Integer)**                  | Represent presence/absence of elements (e.g. subsets, states)    |
| 📊 **BitSet** (Java)                      | Space-optimized boolean array (like `boolean[]`, but compressed) |
| 📄 **String**                             | Convert binary form, manipulate bits as characters               |
| 🧮 **Queue / Stack**                      | Occasionally used with BFS/DFS + bitmask states                  |
| 📈 **Trie (Binary Trie)**                 | Store binary representation of numbers (used in max XOR queries) |


