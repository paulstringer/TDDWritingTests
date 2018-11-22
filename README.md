# STEPS

*A reproduction of an excercise taken from Working with Legacy Code, Chapter 8, Michael Feathers that introduces TDD.*

1. Write a failing test for the first moment about point

	> Given adding elements 1.0 and 2.0. The first moment about point 2.0 should be -0.5.

2. Make it Pass

3. Write a failing test for divide by zero errors

	> Given no elements getting the first moment around point n should thrown an InvalidBasisError

4. Make it Pass

5. Write a failing test for the second moment about point

	> Given adding elements 1.0 and 2.0. The second moment about point 2.0 should be 0.5

	
	Nth Statistic Moment expression for second moment about 2.0
	```
	numerator += Math.pow(element - point, 2.0)
	```

	
6. Make it Pass

7. Remove duplication

8. Clean up the tests for readbility

9. Can we make the tests faster, convert to Logic Tests
