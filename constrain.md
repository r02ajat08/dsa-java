if conatrain the  < 10^5 means 100,000 then o(n) and o(n*log n) will work, avoid using o(n^2) it will give tle 


if maximum operation limit is 10^7

  if input is 

   n<20   that means here 2^n(brute force), n! (back tracking )
   n<3000                 n^2 (dynamic programming)
   3000<n<10^6            O(n), O(n log n) (2 poiner, greedy, heap, sorting)
   n>10^6                 O(log n), o(1)  ( Binary search , math)
