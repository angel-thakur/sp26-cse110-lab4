# Lab 4, Part 1 Answers

1. This line prints "values added: 20"  since add is guaranteed to be true in that block.
2. This line would print "final result: 20" because var defines the variable for the whole scope of the function, thus even though result is not defined in the block with line 13, that line of code can still access it.
3. Var should not be used because it makes variable naming confusing. It may be that you define a variable in a small block at one point but want to reuse the name later and instead of seeing an error, the code silently changes functionality without alerting the developer. This can cause several issues in production and debugging in large codebases. 
4. Line 9 would print "values added: 20" because result is defined as the sum of num1 and num2 in the block that executes when add is true.
5. This would throw an error because since let only defines the variable in the scope of the block/{}, the variable result does not exist at line 13, which is in a different block than the one result is defined in. 
6. This line would throw an error because the const keyword indicates the behavior that whatever value the variable is first assigned to cannot be changed. By trying to change result to num1+num2, the developer is trying to change a const variable, which is not allowed. Thus line 9 is never run since the exception is thrown before this.
7. Since the exception is thrown upon reassigning result to num1+num2, this line would not execute at all.