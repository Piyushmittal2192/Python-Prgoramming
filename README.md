## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/Piyushmittal2192/Python-Prgoramming/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### HackerRank
#### Prob 1: Finding the percentage

You have a record of N students. Each record contains the student's name, and their percent marks in Maths, Physics and Chemistry. The marks can be floating values. The user enters some integer N followed by the names and marks for N students. You are required to save the record in a dictionary data type. The user then enters a student's name. Output the average percentage marks obtained by that student, correct to two decimal places. <br> 

<b>Input Format</b><br> 
The first line contains the integer N, the number of students. The next N lines contains the name and marks obtained by that student separated by a space. The final line contains the name of a particular student previously listed.<br> 

<b>Sample Input</b> <br> 
3 <br> 
Krishna 67 68 69 <br> 
Arjun 70 98 63 <br>
Malika 52 56 60 <br>
Malika <br> 

<b>Sample Output </b> <br> 
56.00
<b>Solution</b> <br>
```markdown
if __name__ == '__main__':
    n = int(input())
    student_marks = {}
    for _ in range(n):
        name, *line = input().split()
        scores = list(map(float, line))
        student_marks[name] = scores
    query_name = input()
    total = 0
    for marks in student_marks[query_name]:
        total = total + marks
    
    avg = total/3.0
    print("{:.2f}".format(avg))
```

```markdown
- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Piyushmittal2192/Python-Prgoramming/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
