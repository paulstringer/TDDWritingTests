# STEPS

*A reproduction of an excercise taken from Working with Legacy Code, Chapter 8, Michael Feathers that introduces TDD.*

This excercise is based on [a simple statistical calculation](https://www.statisticshowto.datasciencecentral.com/what-is-a-moment/), the details of which are not particularly relevant to the excercise.

1. Write a failing test for the first moment about point

	> Given adding elements 1.0 and 2.0. The first moment about point 2.0 should be -0.5.
	
		
	Statistic Moment expression for second moment about 1.0
	
	```
	var numerator = 0.0;

        elements.forEach { (element) in

            numerator += pow(element - point, 1.0)

        }

        return numerator / Double(elements.count)
	```

2. Make it Pass

3. Write a failing test for divide by zero errors

	> Given no elements getting the first moment around point n should thrown an InvalidBasisError

4. Make it Pass

5. Write a failing test for the second moment about point

	> Given adding elements 1.0 and 2.0. The second moment about point 2.0 should be 0.5
	
6. Make it Pass

7. Remove duplication

8. Clean up the tests for readbility

9. Can we make the tests faster, convert to Logic Tests
