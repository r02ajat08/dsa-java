 What is Sliding Window?
Sliding Window is an efficient technique used to reduce nested loops into a single pass. It's most useful in problems involving contiguous subarrays or substrings.

🔹 Types of Sliding Window
Type	Used For
Fixed-size	Problems asking about subarrays of exact size k
Variable-size	Problems asking for longest/shortest subarrays based on a condition

✅ EXAMPLES WITH CODE
📘 Example 1: Fixed-size Sliding Window
Problem:

Find the maximum sum of a subarray of size k.

Input: arr = [1, 4, 2, 10, 23, 3, 1, 0, 20], k = 4
Output: 39
Explanation: Maximum sum = 10 + 23 + 3 + 1 = 37

Approach:

First window: sum first k elements.

Slide window: subtract the element going out, add the element coming in.

Track max.

Java Code:

java
Copy
Edit
public class MaxSumSubarray {
    public static int maxSum(int[] arr, int k) {
        int windowSum = 0;
        int maxSum = 0;

        // sum of first window
        for (int i = 0; i < k; i++) {
            windowSum += arr[i];
        }

        maxSum = windowSum;

        // slide the window
        for (int i = k; i < arr.length; i++) {
            windowSum += arr[i] - arr[i - k];
            maxSum = Math.max(maxSum, windowSum);
        }

        return maxSum;
    }

    public static void main(String[] args) {
        int[] arr = {1, 4, 2, 10, 23, 3, 1, 0, 20};
        int k = 4;
        System.out.println("Max sum of subarray = " + maxSum(arr, k));
    }
}
📘 Example 2: Variable-size Sliding Window
Problem:

Find the smallest subarray length with a sum ≥ target.

Input: arr = [2,3,1,2,4,3], target = 7
Output: 2
Explanation: Subarray [4,3] is the smallest.

Approach:

Use two pointers (start and end)

Expand end to increase the sum.

When sum ≥ target, try to shrink from start.

Java Code:

java
Copy
Edit
public class MinSubArrayLength {
    public static int minSubArrayLen(int target, int[] nums) {
        int minLength = Integer.MAX_VALUE;
        int left = 0, sum = 0;

        for (int right = 0; right < nums.length; right++) {
            sum += nums[right];

            while (sum >= target) {
                minLength = Math.min(minLength, right - left + 1);
                sum -= nums[left++];
            }
        }

        return minLength == Integer.MAX_VALUE ? 0 : minLength;
    }

    public static void main(String[] args) {
        int[] nums = {2, 3, 1, 2, 4, 3};
        int target = 7;
        System.out.println("Min subarray length = " + minSubArrayLen(target, nums));
    }
}
📘 Example 3: Longest Substring Without Repeating Characters
(Classic variable window for strings)

Input: "abcabcbb"
Output: 3 ("abc")

Approach:

Use Set to track characters.

Expand right pointer until duplicate.

Then move left until the duplicate is removed.

Java Code:

java
Copy
Edit
import java.util.HashSet;

public class LongestUniqueSubstring {
    public static int lengthOfLongestSubstring(String s) {
        int left = 0, right = 0, maxLen = 0;
        HashSet<Character> seen = new HashSet<>();

        while (right < s.length()) {
            if (!seen.contains(s.charAt(right))) {
                seen.add(s.charAt(right));
                maxLen = Math.max(maxLen, right - left + 1);
                right++;
            } else {
                seen.remove(s.charAt(left));
                left++;
            }
        }

        return maxLen;
    }

    public static void main(String[] args) {
        String s = "abcabcbb";
        System.out.println("Longest unique substring = " + lengthOfLongestSubstring(s));
    }
}
🧠 Pattern Summary
Problem Type	Window Type	Data Structures
Max sum of subarray of size k	Fixed-size	Variables
Min subarray length with sum ≥ target	Variable-size	Two pointers + sum
Longest unique substring	Variable-size	Set / Map
