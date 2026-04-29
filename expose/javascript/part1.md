1. values added: 20
2. final result: 20
3. Here we shouldn't use ```var``` because ```var``` means the variable ```result``` is function scoped instead of block scoped. This means that ```result``` is still accessible outside of the ```if``` statement which completely voids the use of an ```if``` statement in this case.
4. values added: 20
5. It would return an error because ```let``` means that ```result``` is block scoped and ```result``` is not defined outside of the if statement.
6. It would cause an error because the line ```result = num1 + num2;``` is changing ```result``` after declaring it. This violates the ```const``` call for the variable.
7. It would cause an error for the same reason as #6. Also, ```const``` means that it's block scoped and this is calling it outside of the block where ```result``` is defined.