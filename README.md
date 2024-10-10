# SWE_2021_41_2024_2_week_6
---
**Week 4 Assignment** 
* https://github.com/Laqwuirr/SWE_2021_41_2024_2_week_4
<pre>
  <code>
def isHappy(n):
    seen = set()

    sum = 0
    while sum != 1:
      sum = 0
      for digit in str(n):
        sum += int(digit) ** 2

      #print("Sum: ", sum)
      n = sum

      if sum in seen:
        return False
      seen.add(sum)

    if sum == 1:
      return True

n = int(input())
print(isHappy(n))

  </code>
</pre>
*
