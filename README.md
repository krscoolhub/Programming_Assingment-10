# Programming_Assingment-10


1. Write a Python program to find sum of elements in list?
sol:
l = [2, 4, 1, 5, 6, 7]

total = 0
for i in l:
    total += i
    
print(total)
25




2. Write a Python program to Multiply all numbers in the list?
sol:
l = [2, 4, 1, 5, 6, 7]

mul = 1
for i in l:
    mul *= i
    
print(mul)
1680



3. Write a Python program to find smallest number in a list?
sol:
l = [2, 0, 1, 1235, 6, -7123]

minimum = l[0]
for i in l:
    if i < minimum:
        minimum = i
        
print(minimum)
-7123




4. Write a Python program to find largest number in a list?
sol:
l = [2, 0, 1, 1235, 6, -7123]

maximum = l[0]
for i in l:
    if i > maximum:
        maximum = i
        
print(maximum)
1235




5. Write a Python program to find second largest number in a list?
sol:
l = [2, 0, 1, 1235, 6, -7123]
l.sort(reverse=True)
print("Second largest number:", l[1])
Second largest number: 6




6. Write a Python program to find N largest elements from a list?
sol:
def findLarge(lst, n):
    
    lst.sort(reverse = True)
    return lst[n-1]
# 2nd Largest Element

l = [2, 0, 1, 1235, 6, -7123]
findLarge(l, 2)
6
# 4th Largest Element

l = [2, 0, 1, 1235, 6, -7123]
findLarge(l, 4)
1




7. Write a Python program to print even numbers in a list?
sol:
l = [2, 0, 1, 1235, 6, -7123, 21, 54, 12, -23, -42]

[ i for i in l if i%2 == 0]
[2, 0, 6, 54, 12, -42]




8. Write a Python program to print odd numbers in a List?
sol:
l = [2, 0, 1, 1235, 6, -7123, 21, 54, 12, -23, -42]

[ i for i in l if i%2 == 1]
[1, 1235, -7123, 21, -23]




9. Write a Python program to Remove empty List from List?
sol:
l = [[], 12, 31, [1,2, -23] , [1], [], [123.23], [], 2, 321]

result = []
for i in l:
    if type(i) == list:
        if len(i) != 0:
            result.append(i)
    else:
        result.append(i)

result
            
            
[12, 31, [1, 2, -23], [1], [123.23], 2, 321]



10. Write a Python program to Cloning or Copying a list?
sol:
list1 = [2,1, 31, 3, 412, 3, 4667, [2,3,1]]
list2 = []

for i in list1:
    list2.append(i)
    
print(list2)
[2, 1, 31, 3, 412, 3, 4667, [2, 3, 1]]




11. Write a Python program to Count occurrences of an element in a list?
sol:
l = [1,1,1, 3, 4, 1, 7, 8, 6,6,2,1]

def occurrences(lst, element):
    count = 0
    for i in lst:
        if i == element:
            count += 1
            
    return count
occurrences(l, 1)
5




def occurrences(lst, element):
    count = 0
    for i in lst:
        if i == element:
            count += 1
            
    return count
occurrences(l, 1)
5
