# Edna's Lab Report 5 Week 10

In week 9, we practiced using vimdiff to display the differences between the outputs of two different MarkdownParse files. The format of the output between the two were the same because we used the same script.sh file as well as the same test-file folder of tests for both.

To remotely find the different results, used vim to edit the script.sh file to include the file names before its specific output from the TA's cloned repository. I then put the output in a file called "taresults.txt". Then, I cloned my own repository for MarkdownParse in a folder called lab9markdown-parse. I copied the script.sh and test-files folder from the TA's repository onto my own repository. After running ```bash script.sh``` to see if it's running, I moved my own results into a folder called "myresults.txt". Finally, I used ```vimdiff cse15lsp22-markdown-parser/taresults.txt lab9markdown-parse/myresults.txt ``` to display the two outputs side by side. By doing so, I can see the highlighted lines where the outputs are different. 

**Two Tests Files With Different Outputs**

[Test File 573](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/573.md)

[Test File 577](https://github.com/nidhidhamnani/markdown-parser/blob/main/test-files/577.md)

My implementation is correct for each output. 
