# Markdown to HTML

## Description
> Markdown is awesome! All your README.md are made in Markdown, but do you know how GitHub are rendering them?

> It’s time to code a Markdown to HTML!

### Requirements
1. All your files will be interpreted/compiled on Ubuntu 18.04 LTS using python3 (version 3.7 or higher)
2. The first line of all your files should be exactly #!/usr/bin/python3
3. A README.md file, at the root of the folder of the project, is mandatory
4. Your code should use the PEP 8 style (version 1.7.*)
5. All your files must be executable
6. All your modules should be documented: python3 -c 'print(__import__("my_module").__doc__)'
7. Your code should not be executed when imported (by using if __name__ == "__main__":)

#### Tasks
0. Start a script
#advanced
Write a script markdown2html.py that takes an argument 2 strings:

First argument is the name of the Markdown file
Second argument is the output file name
Requirements:

If the number of arguments is less than 2: print in STDERR Usage: ./markdown2html.py README.md README.html and exit 1
If the Markdown file doesn’t exist: print in STDER Missing <filename> and exit 1
Otherwise, print nothing and exit 0


1. Headings
#advanced
Improve markdown2html.py by parsing Headings Markdown syntax for generating HTML:

Syntax: (you can assume it will be strictly this syntax)

Markdown	HTML generated
# Heading level 1	<h1>Heading level 1</h1>
## Heading level 2	<h2>Heading level 1</h2>
### Heading level 3	<h3>Heading level 1</h3>
#### Heading level 4	<h4>Heading level 1</h4>
##### Heading level 5	<h5>Heading level 1</h5>
###### Heading level 6	<h6>Heading level 1</h6>


2. Unordered listing
#advanced
Improve markdown2html.py by parsing Unordered listing syntax for generating HTML:

Syntax: (you can assume it will be strictly this syntax)

Markdown:- Hello
- Bye
HTML generated:

<ul>
    <li>Hello</li>
    <li>Bye</li>
</ul>


3. Ordered listing
#advanced
Improve markdown2html.py by parsing Ordered listing syntax for generating HTML:

Syntax: (you can assume it will be strictly this syntax)


4. Simple text
#advanced
Improve markdown2html.py by parsing paragraph syntax for generating HTML:

Syntax: (you can assume it will be strictly this syntax)

Markdown:
Hello

I'm a text
with 2 lines
HTML generated:

<p>
    Hello
</p>
<p>
    I'm a text
        <br />
    with 2 lines
</p>


5. Bold and emphasis text
#advanced
Improve markdown2html.py by parsing bold syntax for generating HTML:

Syntax: (you can assume it will be strictly this syntax)

Markdown	HTML generated
**Hello**	<b>Hello</b>
__Hello__	<em>Hello</em>



6. ... but why??
#advanced
Improve markdown2html.py by parsing bold syntax for generating HTML:

Syntax: (you can assume it will be strictly this syntax)

Markdown	HTML generated	description
[[Hello]]	8b1a9953c4611296a827abf8c47804d7	convert in MD5 (lowercase) the content
((Hello Chicago))	Hello hiago	remove all c (case insensitive) from the content

