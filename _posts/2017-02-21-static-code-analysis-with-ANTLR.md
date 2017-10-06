---
title: Static Code Analysis With ANTLR
updated: 2017-02-21 18:30
categories:
    - software-development
---
This is a short write-up about my first experiences with the [ANTLR framework](http://www.antlr.org/) and its use for static code analysis.  
- - -
At the start of my third semester I took a course about Software Development. This course consisted of a group project, for which I was the project leader as well as a developer. The goal was to redesign an older project, the "CodeInspector" which, as you might have already guessed, which inspects code by analyzing it class by class. After the analysis you get a grade and a set of remarks about your code.  
My job, other than organizing the group, was to write a parser that recognizes C and Java and is easy to extend to read other programming languages.   

After doing some research I found the ANTLR framework, which seemed to be a perfect match. With a some knowledge of grammars it was relatively easy to understand. I found that [this tutorial](https://theendian.com/blog/antlr-4-lexer-parser-and-listener-with-example-grammar/) was a very good start and helped me out massively.  
Luckily there were mostly bug-free [grammars](https://github.com/antlr/grammars-v4) for many languages in the ANTLR project from which I used Java and C.  
Most of the "thinking work" went into the semantic models and DTOs(Data Transfer Objects) as well as the listeners. Here's some insight into the parser's architecture:  

![classDiagram]({{site.baseurl}}/assets/images/Klassendiagramm_Parser.png)  

Looking back, most of the actual work was needed to understand and the existing grammars and finding the right rules, subrules etc. from which the correctly scoped information could be extracted. Luckily we managed to avoid using a symbol table, keeping the complexity fairly low.  

Somehow we managed to win second place in a university-internal [competition](https://www.hft-leipzig.de/de/hochschule/aktuelles/swe-2017.html), the prize being a very insightful workshop in penetration testing. 
