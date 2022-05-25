# Edna's Lab Report 4 Week 8

For the past few weeks, we've been looking into testing our code with JUnit tests and debugging according to any error messages. For MarkdownParse, I have my own implementation as well as another peer's implementation. We'll be testing each implementation with given test files to see if our implementations account for the situations.

[link to my markdown-parse directory](https://github.com/ednavho/ednafiles.git)

[link to my peer's markdown-parse directory](https://github.com/ednavho/bellamarkdown.git)

## **Test Snippet 1**

- The expected output should be:

    ```[`google.com, google.com, ucsd.edu]```
    
- The test in MarkdownParseTest.java for each implementation should look like this:

![myimptest1](myimptest1.png)

- The corresponding output when running the JUnit test with my implementation:

![myimptest1output](myimpytest1output.png)

- The corresponding output when running the JUnit test with my peer's implementation:

![bellatest1output](bellatest1output.png)


## **Test Snippet 2**

- The expected output should be:

    ```[a.com, a.com(()), example.com]```
    
- The test in MarkdownParseTest.java for each implementation should look like this:

![myimptest2](myimptest2.png)

- The corresponding output when running the JUnit test with my implementation:

![myimptest2output](myimptest2output.png)

- The corresponding output when running the JUnit test with my peer's implementation:

![bellatest2output](bellatest2output.png)


## **Test Snippet 3**

- The expected output should be:

    ```[https://sites.google.com/eng.ucsd.edu/cse-15l-spring-2022/schedule]```
    
- The test in MarkdownParseTest.java for each implementation should look like this:

![myimptest3](myimptest3.png)

- The corresponding output when running the JUnit test with my implementation:

![myimptest3output](myimp3output.png)

- The corresponding output when running the JUnit test with my peer's implementation:

![bellatest3output](bella3output.png)


## **Debugging Ideas**

1. For test snippet 1, a code change could be done in less than 10 lines. After it checks for the bracket and parenthesis indices, it should check for ticks, and any existing pair of ticks near brackets should be within the pair of brackets. After checking for the closing bracket, it should check if there's another closing bracket to see if that one should be the end of the link name. 

2. For test snippet 2, a code change could be done in less than 10 lines. After checking for a certain punctuation, it should check if a duplicate follows somewhere after and update a count for that specific punctuation. Unless, it follows the case that the closing bracket and opening parenthesis are right next to each other, it should only consider the outer punctuations as the outmost link formatting.

3. For test snippet 3, a code change could be done in less than 10 lines. While checking for correct link format, the code should not only check if the link contains spaces, but it should also check for entire line breaks within the brackets. If it has any of these, the if statement should continue to after the closed parenthesis.

