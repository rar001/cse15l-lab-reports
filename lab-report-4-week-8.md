# Lab Report Week 8!
![title](/labreport4/lab7.png)

---
## Links to Repos

[Link to My Repository](https://github.com/rar001/markdown-parser)

[Link to Reviewees Repository](https://github.com/aHewig/markdown-parser)

I will segment this lab report by the 3 snippets we were tasked with testing.

*I based the valid links off of [CommonMark](https://spec.commonmark.org/dingus/).* 


## Snippet 1
The following is the code for turning Snippet 1 into a test on my file, followed by the same process for the other user's file.

My File:
![mysnippet1code](/labreport4/mysnippet1code.png)

---

Other File:
![othersnippet1code](/labreport4/othersnippet1code.png)

Next, I will show the running test for Snippet 1 in my file, followed by the running test for the other user's file.

My File with JUnit Test Failure:
![mysnippet1test](/labreport4/mysnippet1test.png)

---

Other File with JUnit Test Failure:
![othersnippet1test](/labreport4/othersnippet1test.png)


## Snippet 2
The following is the code for turning Snippet 2 into a test on my file, followed by the same process for the other user's file.

My File:
![mysnippet2code](/labreport4/mysnippet2code.png)

---

Other File:
![othersnippet2code](/labreport4/othersnippet2code.png)

Next, I will show the running test for Snippet 2 in my file, followed by the running test for the other user's file.

My File with JUnit Test Failure:
![mysnippet2test](/labreport4/mysnippet2test.png)

---

Other File with JUnit Test Failure:
![othersnippet2test](/labreport4/othersnippet2test.png)


## Snippet 3
The following is the code for turning Snippet 3 into a test on my file, followed by the same process for the other user's file.

My File:
![mysnippet3code](/labreport4/mysnippet3code.png)

---

Other File:
![othersnippet3code](/labreport4/othersnippet3code.png)

Next, I will show the running test for Snippet 3 in my file, followed by the running test for the other user's file.

My File with JUnit Test Failure:
![mysnippet3test](/labreport4/mysnippet3test.png)

---

Other File with JUnit Test Failure:
![othersnippet3test](/labreport4/othersnippet3test.png)


# Questions
## Question 1
I don't think that there is a code change that is less than 10 lines that could account for Snippet 1 backticks. I think that it would be more involved because you would have to account for backticks for every situation like, backticks within the url title, backticks within the actual url, backticks that occur both in and out of the url. All of these edge cases would need to be accounted for.

## Question 2
I don't think that there is a code change that is less than 10 lines that could account for Snippet 2 overlapping parenthesis, brackets, etc. This is because there are endless edge cases to account for. There is not any quick solution to this that my knowledge could fill.

## Question 3
I believe there may be a code change that is less than 10 lines for URLs that take up new lines. I think there could be a cut off limit for the length of URLs, and if the space between the start of the URL and the end of the URL is too great, the program could not include it in the link list. Something like:

`if (text.indexOf(closedBracket) - text.indexOf(openBracket) > 25) {`

`currentIndex = text.indexOf(closedBracket) + 1;`

`}`