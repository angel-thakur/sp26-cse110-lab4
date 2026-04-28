# Lab 4, Part 2 Answers

1. This would print the value 3. It does not cause an error because var can be redefined and i exists across the whole function.
2. A similar thing would happen at line 13. Since discountedPrice exists in that scope, it would print 150.
3. The finalPrice at the end of the loop is the same as discountedPrice which is reachable due to var's scope. It would print 150.
4. This would return the array [50, 100, 150] because at each index, the previous sum is overwritten and the current discounted price is correctly added to the array discounted, which has scope throughout the function


5. This would be an error because due to let's scope, i does not exist at the console call.
6. This would be an error because due to let's scope, discountedPrice does not exist at the console call.
7. This would not be an error because discountedPrice is declared at the beginning of the function in the same block as the console call, so when that line runs, it has access to the variable, printing 150.
8. This would also return the array [50, 100, 150]. Even though the variables are inaccessible at the point of return, the values of the computation are all stored in the array discounted, which is accessible.

9. An error would happen because let i means that i is not accessible outside the scope of the for loop.
10. This variable does not change and it was declared in the scope its being accessed in, so it prints 3.
11. This also returns the right answer in the end because const can be redelcared, just not changed and this implementation does not change const. Thus all the correct values are returned in array [50, 100, 150]

12.  
     - student.name
     - student['Grad Year']
     - student.greeting()
     - student['Favorite Teacher'].name
     - student.courseLoad[0]
13.  
    - '32' because string concatenation is triggered
    - 1 because - converts to a number
    - 3 because null becomes 0 in numerical operations
    - '3null' because string concatenation is triggered
    - 4 because true is interpreted as 1
    - 0 because false = 0 and null = 0 and 0+0=0
    - '3undefined' because string concatenation is triggered
    - 
14.  
    - True because '2' is coverted to number
    - False because both are strings ad '2' is not lexicographically larger than '1'
    - True because '2' is coverted to number
    - False because === checks number and type
    - False because true = 1 != 2
    - True because Boolean(2) = true
15. == does not check types before comparing while === does. Both the type and value must match for the latter to be true while only the value must be equal for the former to be true.

16.    
for (let property in statistics) {
  if (property.startsWith('r') || statistics[property] % 2 !== 0) {
    console.log(statistics[property]);
  }
}

17. The result should be [2, 4, 6] because for every index of the input array, we apply the callback, which returns the input times 2. Then we push it to our function-scope vairable newArr. Thus, the function should multiply each index of the input array by 2. 
18.    
setInterval(() => {
  const d = new Date();
  console.log(d.toLocaleTimeString());
}, 1000);
19. 1, 4, 3, 2