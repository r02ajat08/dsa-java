
# 📚✨ DSA Array Patterns – Cheat Sheet with Time ⏱ & Space 💾 Complexities

| 🔢 | 🧠 Pattern / Algorithm              | ⏱️ Time Complexity      | 💾 Space Complexity   | 🔍 Use Case Keywords |
|----|-----------------------------------|--------------------------|------------------------|----------------------|
| 1️⃣ | 🔄 **Sliding Window**             | `O(n)`                   | `O(1)` / `O(k)`        | 📏 Subarray, sum, average, max/min window |
| 2️⃣ | 🎯 **Two Pointers**               | `O(n)`                   | `O(1)`                 | 🎯 Sorted array, pair sum, reverse, move zeroes |
| 3️⃣ | ➕ **Prefix Sum / Difference**    | `O(n)`                   | `O(n)`                 | 🧮 Range sum, subarray sum, balanced array |
| 4️⃣ | 🧠 **Hashing (Map / Set)**        | `O(n)`                   | `O(n)`                 | 🔍 Frequency, duplicates, lookup, anagrams |
| 5️⃣ | 🔃 **Sorting**                    | `O(n log n)`             | `O(1)` to `O(n)`       | 🗂️ Order elements, intervals, greedy prep |
| 6️⃣ | 💡 **Greedy**                     | `O(n)` or `O(n log n)`   | `O(1)`                 | ⚡ Pick best option at every step, jobs, coins |
| 7️⃣ | 🧮 **Binary Search**              | `O(log n)` / `O(log max)`| `O(1)`                 | 🎯 Search position, peak element, rotation |
| 8️⃣ | 📏 **Monotonic Stack / Queue**   | `O(n)`                   | `O(n)`                 | 📊 NGE, stock span, sliding window max |
| 9️⃣ | 🔢 **Bit Manipulation**           | `O(n)`                   | `O(1)`                 | 💡 XOR, set bits, power of 2, bitmask |
| 🔟  | 🔁 **Backtracking**               | `O(2^n)` / `O(n!)`       | `O(n)`                 | 🌀 Subsets, permutations, combinations |
| 1️⃣1️⃣ | 📈 **Kadane’s Algorithm**         | `O(n)`                   | `O(1)`                 | 💥 Max subarray sum |
| 1️⃣2️⃣ | ⚔️ **Divide & Conquer**           | `O(n log n)`             | `O(log n)`             | 🧩 Merge sort, max subarray, binary tricks |
| 1️⃣3️⃣ | 🚦 **Dutch National Flag Algo**   | `O(n)`                   | `O(1)`                 | 🎨 Sort 0s, 1s, 2s / 3-way partition |
| 1️⃣4️⃣ | 🌀 **Fast & Slow Pointers**       | `O(n)`                   | `O(1)`                 | 🔄 Cycle detection, repeated numbers |

---

## 🎯 Quick Pattern Matching

| 🧩 Problem Says...                  | 💡 Use This Pattern         |
|------------------------------------|-----------------------------|
| "Find max/min in subarray"         | 🔄 Sliding Window           |
| "Pair with sum / diff / product"   | 🎯 Two Pointers or Hashing  |
| "Range sum / subarray = k"         | ➕ Prefix Sum               |
| "Frequency, duplicates, lookup"    | 🧠 HashMap / HashSet        |
| "Find position, rotation, peak"    | 🧮 Binary Search            |
| "Next Greater Element / Stock"     | 📏 Monotonic Stack          |
| "Unique subset / permutation"      | 🔁 Backtracking             |
| "Cycle / repeated value"           | 🌀 Fast & Slow Pointers     |
| "Optimal choice at every step"     | 💡 Greedy                  |
| "Sort or merge recursively"        | ⚔️ Divide & Conquer        |
