
<!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->

<!-- code_chunk_output -->

- [Text and link](#text-and-link)
- [Blockquote](#blockquote)
- [Emphasis](#emphasis)
- [Horizontal Rule](#horizontal-rule)
- [Miscellaneous](#miscellaneous)
- [List](#list)
- [To-do List/Tasks list](#to-do-listtasks-list)
- [Style Code](#style-code)
- [Flow Charts](#flow-charts)
- [Sequence Diagrams](#sequence-diagrams)
- [Tables](#tables)
- [Mathematical formula \(y = x^2\)](#mathematical-formula-y--x2)

<!-- /code_chunk_output -->

### Text and link
It's very easy to make some words **bold** and other words *italic* with Markdown. Any word wrapped with two tildes (like ~~this~~) will appear crossed out. 
You can even [link to Google!](http://google.com)
And, of course emoji! :sparkles: :camel: :boom:
If you want to embed images, this is how you do it:
![Image of Yaktocat](https://octodex.github.com/images/yaktocat.png)
*注：插入图片的语法和链接的语法很像，只是前面多了一个 ！*

### Blockquote
If you'd like to quote someone, use the > character before the line:

As Kanye West said:
> We're living the future so
> the present is our past.

### Emphasis
*This text will be italic*
_This will also be italic_

**This text will be bold**
__This will also be bold__

_You **can** combine them_

~~This text will be strikethrough~~

### Horizontal Rule
Three or more...
Hyphens`---`

---
Asterisks`***`
***
Underscores`___`
___

### Miscellaneous
- Footnotes 
  Content [^1]
  [^1]: Hi! This is a footnote
- Superscript 
  30^th^
- Subscript 
  H~2~O
- Abbreviation
  The HTML specification is maintained by the W3C.
  *[HTML]: Hyper Text Markup Language
  *[W3C]:  World Wide Web Consortium
- Mark 
  ==marked==

### List
Numbered lists:
1. One
2. Two
3. Three

Bullet points:
* Start a line with a star
* Profit!

Alternatively,
- Dashes work just as well
- And if you have sub points, put two spaces before the dash or star:
  - Like this
  - And this

### To-do List/Tasks list
- [x] 已完成项目1
    - [x] 已完成事项1
    - [ ] 待办事项2
- [ ] 待办项目2
- [ ] 待办项目3

### Style Code
Inline code blocks, wrap them in backticks: `var example = true`.  

Indent with four spaces:

    if (isAwesome){
      return true
    }

Code fencing, which allows for multiple lines without indentation:

```
if (isAwesome){
  return true
}
```

Syntax highlighting with line numbers:

```python {.line-numbers}
#!/usr/bin/python

class Employee:
   'Common base class for all employees'
   empCount = 0

   def __init__(self, name, salary):
      self.name = name
      self.salary = salary
      Employee.empCount += 1
   
   def displayCount(self):
     print "Total Employee %d" % Employee.empCount

   def displayEmployee(self):
      print "Name : ", self.name,  ", Salary: ", self.salary

"This would create first object of Employee class"
emp1 = Employee("Zara", 2000)
"This would create second object of Employee class"
emp2 = Employee("Manni", 5000)
emp1.displayEmployee()
emp2.displayEmployee()
print "Total Employee %d" % Employee.empCount
```

### Flow Charts
```flow
st=>start: Start|past:>http://www.google.com[blank]
e=>end: End|future:>http://www.google.com
op1=>operation: My Operation|past
op2=>operation: Stuff|current
sub1=>subroutine: My Subroutine|invalid
cond=>condition: Yes
or No?|approved:>http://www.google.com
c2=>condition: Good idea|rejected
io=>inputoutput: catch something...|future
st->op1(right)->cond
cond(yes, right)->c2
cond(no)->sub1(left)->op1
c2(yes)->io->e
c2(no)->op2->e
```

### Sequence Diagrams
```sequence {theme="hand"}
Title: Here is a title
A->B: Normal line
B-->C: Dashed line
C->>D: Open arrow
D-->>A: Dashed open arrow
```

### Tables
| First Header                | Second Header                |
| --------------------------- | ---------------------------- |
| Content from cell 1         | Content from cell 2          |
| Content in the first column | Content in the second column |

### Mathematical formula \(y = x^2\)
Inline math: $\dfrac{ \tfrac{1}{2} [1-(\tfrac{1}{2})^n] }{ 1-\tfrac{1}{2} } = s_n$.

Math block:
```math
\oint_C x^3\, dx + 4y^2\, dy
```
$$ 2 = \left( \frac{\left(3-x\right) \times 2}{3-x} \right) $$

$$ \sum_{m=1}^\infty \sum_{n=1}^\infty \frac{m^2\, n} {3^m\left(m\, 3^n+n\, 3^m\right)}
 $$

\[\phi_n(\kappa) = \frac{1} {4\pi^2\kappa^2} \int_0^\infty \frac{\sin(\kappa R)}{\kappa R} \frac{\partial}{\partial R} \left[R^2\frac{\partial D_n(R)}{\partial R}\right]\, dR\]
