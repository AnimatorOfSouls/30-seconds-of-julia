---
title: fact
tags: math,beginner
---

Calcaultes the factorial of a number.

Calculates num * factorial of num-1. Once the program reaches the factorial of 0, the function returns 1,
thus allowing the function to calculate each of the factorials up to the input number.

```jl
function fact(num)
  if num < 0
    println("The number needs to be greater than or equal to zero.")
    return
    
  else
    if num == 0
      return 1
      
    else
      num = num*fact(num-1)
      return num
    end
  end
end
```

```jl
fact(4) # 24
```
