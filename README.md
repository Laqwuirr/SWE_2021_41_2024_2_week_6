# SWE_2021_41_2024_2_week_6
---
### **Week 4 Assignment**
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
* The function “isHappy” determines whether a given number is a happy number. A happy number is a number that, after repeating a certain process, eventually leads to 1.

  1. Starting with an input of any positive integer.
  2. The while loop calculates the sum of the squares of the digits of the current number n. It works until the sum is not equal to 1.
  3. The current number n is given the value of the sum.
  4. If sum is seen more than once in a loop or the new value of the number is already in the seen set, the function returns False, because it means that it loops endlessly in a cycle which does not include 1.
  5. If the sum equals 1, the function returns True, indicating that the number is happy.
  6. If the number does not reach 1 and does not endlessly loop, we add the sum to the seen set and continue the process.
---
**Week 5 Assignment**
> ```python
> docker exec ossp-container cat /etc/os-release
> ```
> * <u>docker exec:</u> is used to run a command inside a running Docker container. \
cat /etc/os-release: inside the container, the command *cat* shows the contents of */etc/os-release* file which contains the information about the operating system running inside the container *ossp-container*.

<br>
