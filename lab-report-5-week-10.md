## Week 10 Lab Report

# Two Tests

![Two different output tests](Line212and270.PNG)
The two tests I chose for this lab report are tests that produced the output on lines 212 and 270. 

# Explain:
# Part 1
In our lab we found the differences between our outputs using `diff`. We ran the command `diff /home/linux/ieng6/cs15lwi22/cs15lwi22aqe/class-clone/results.txt new-results.txt`
to print out all of the test cases where our code produced a different output from the given code. The diff command compared the outputs that we stored in new-results.txt
in our markdownparse file and the results.txt that we stored in the given markdownparse file. From here we know which line in new-results.txt produced the difference so if we
look inside new-results.txt using vim we can see the output that was different and the corresponding test file that errored above the output.

![Line 212](Line212Test.PNG)

![Line 270](Line270Test.PNG)

Now that we know which tests failed we are able to loop inside these test files and see the problem.

# Part 2

![Test 194](Test194.PNG)
The given code produces the output `url` after running this test.

![Given Code's Issue To Fix](194Problem.PNG)
The expected output from running test 194 is an empty list. This is because test file 194 is not following the format of a file. The issue in the given code is that it is only
looking for open brackets, closing brackets, open parenthesis, and closing parenthesis to exist. It is not checking that the closing bracket is next to the open parenthesis.

![Test 22](Test22.PNG)
Our code produces the `output /bar\* "ti\*tle"` after running this test.

![Our Code's Issue To Fix](22Problem.PNG)
The expected output from running test 22 is an empty list. This is because there is a space inside the parenthesis in between text. The issue in our code is that we do not check
for spaces in between text inside of our links. We can fix this by adding an if statement before we add the potential link to our list.