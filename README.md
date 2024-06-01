# Offer-Time

Yash is ordering food online and the bill comes out to be Rs. X. Yash can use one of the following two coupons to avail a discount.
 1. Get 10 percent off on the bill amount
 2. Get a flat discount of Rs. 100 on the bill amount
What is the maximum discount Yash can avail ?

Input
The first and only line contains a single integer X - the bill amount before discount.

Constraints
100 ≤ X ≤ 10000
X is a multiple of 100.
Output
Print the maximum discount Yash can avail.

def maximum_discount(X):
    discount_10_percent = X * 0.10
    
    flat_discount = 100
    
    max_discount = max(discount_10_percent, flat_discount)
    
    return int(max_discount)

X = int(input().strip())
print(maximum_discount(X))
