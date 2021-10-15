1) It should print ~~prices.length~~ 3, since i has been iterated until it reaches that number. Then the for loop stops, and i remains having that value.
2) It should print ~~prices[prices.length-1]\*(1-discount)~~ 150 since the last assignment of discountedPrice will happen at i = prices.length-1
3) It should print ~~Math.round(prices[prices.length-1]\*(1-discount)\*100)/100~~ 150 since the last assignment of finalPrice will happen at i = prices.length-1, and it'll pull that value of discountedPrice.
4) It'll return the array [50,100,150] which is each element of prices adjusted by the discount. 
5) Undefined, since the definition of i is in a smaller scope than that of the console.log statement.
6) Undefined, since the definition of discountedPrice is in a smaller scope than that of the console.log statement.
7) That'll print 150. It works fine because the definition of the scope of finalPrice is on the same level as the console.log statement, and otherwise refer to 3. 
8) I *think* this should return [50,100,150], because the definition of discounted is on the same scope as the return statement, and since javascript doesn't use pointers, the return should clone the array, so it wouldn't be a memory leak. I could be wrong if javascript has some other type of safeguard around their return statement and it'd return undefined istead if the function is trying to pass the returned value outside the scope of where it's defined, but I don't think that's the case. 
9)  Undefined, since the definition of i is in a smaller scope than that of the console.log statement.
10) That'll print 3, since the const is defined on the same scope as the console.log statement.
11) [50,100,150] since the array is fine to be changed, just not reassigned. 
12) Data types
    1)  student.name
    2)  student['Grad Year']
    3)  student.greeting()
    4)  student['Favorite Teacher'].name
    5)  student.courseload[0]
13) Arithmetic
    1)  '32' because 2 is concatenated to string.
    2)  1 because '3' is converted to integer so it can be part of subtraction.
    3)  3 because null is converted to 0 and added.
    4)  '3null' because null is converted to string and concatenated.
    5)  4 because true is converted to 1 and added.
    6)  0 because both false and null are converted to integers and added.
    7)  '3undefined' because undefined is converted to string and concatenated.
    8)  NaN because '3' is converted to an integer and the operation fails because undefined is not a number (NaN)
14) Comparison
    1)  true because both variables are compared as integers
    2)  false because both variables are compared as strings, and '2' has higher precidence than '12' with a higher first character.
    3)  true because both variables are compared as integers
    4)  false because === considers variable type as well, and both integers do not share a type.
    5)  false because both variables are compared as integers, and true is considered 1, so 1 =/= 2. 
    6)  true because the boolean evaluation of 2 is true, so both have condition true.
15) == forces type conversion and then checks for equality (doesn't care about type) and === compares values and type (does care about type).
16) Completed.
17) It'd result in the creation of a new array: [2,4,6] which is instantly lost because it's not assigned to any variable. array is unchanged. 
18) The code I wrote for this did work :D
19) 1342