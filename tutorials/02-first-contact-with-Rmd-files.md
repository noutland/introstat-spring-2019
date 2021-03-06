First contact with Rmd files
================
Gaston Sanchez

> ### Learning Objectives:
> 
>   - Get started with R markdown (Rmd) files
>   - Understand the anatomy of an Rmd file
>   - Get to know markdown syntax
>   - Understand code chunks

## Introduction to Rmd files

In this course, you will be using one main type of source file known as
*R markdown* file, simply referred to as `Rmd` files.

**Rmd** files are a special type of file technically known as *dynamic
documents*. This type of documents allows you to combine narrative
(text) with R code, which means that you write everything (text and
code) in one single file.

### Opening and knitting an `Rmd` file

  - In the menu bar of RStudio, click on **File**
  - Then **New File**, and choose **R Markdown**
  - Select the default option “Document” (HTML output), and click
    **Ok**.
  - Locate **Knit** the button (the one with a knitting icon) and click
    on it so you can see how `Rmd` files are rendered and displayed as
    HTML documents.

### What is an `Rmd` file?

**Rmd** files are a special type of file, referred to as a *dynamic
document*. This is the fancy term we use to describe a document that
allows us to combine narrative (text) with R code in one single file.

The main idea behind dynamic documents is simple yet very powerful:
instead of working with two separate files, one that contains the R
code, and another one that contains the narrative, you use an `.Rmd`
file to include both the commands and the narrative.

One of the main advantages of this paradigm, is that you avoid having to
copy results from your computations and paste them into a report file.
In fact, there are more complex ways to work with dynamic documents and
source files. But the core idea is the same: combine narrative and code
in a way that you let the computer do the manual, repetitive, and time
consuming job.

It is extremeley important that you quickly become familiar with `Rmd`
files. You’ll be using `Rmd` files to write your lab and homework
assignments, and convert them to HTML files (you could also convert them
to Word, or PDF files, among other formats).

### Anatomy of an `Rmd` file

The structure of an `.Rmd` file can be divided in two parts: 1) a **YAML
header**, and 2) the **body** of the document. In addition to this
structure, you should know that `.Rmd` files chiefly use three types of
syntaxes: YAML, Markdown, and R.

The *YAML header* consists of the first few lines at the top of the
file. This header is established by a set of three dashes `---` as
delimiters (one starting set, and one ending set). This part of the file
requires you to use YAML syntax (Yet Another Markup Language.) Within
the delimiter sets of dashes, you specify settings (or metadata) that
will apply to the entire document. Some of the common options are things
like:

  - `title`
  - `author`
  - `date`
  - `output`

The *body* of the document is everything below the YAML header. It
consists of a mix of narrative and R code. All the text that is
narrative is written in a markup syntax called **Markdown** (although
you can also use LaTeX math notation). In turn, all the text that is
code is written in R syntax inside *blocks of code*.

There are two types of blocks of code: 1) **code chunks**, and 2)
**inline code**. Code chunks are lines of text separated from any lines
of narrative text. Inline code is code inserted within a line of
narrative text .

### How does an Rmd file work?

Rmd files are plain text files. All that matters is the syntax of its
content. The content is basically divided in the header, and the body.

  - The header uses YAML syntax.
  - The narrative in the body uses Markdown syntax.
  - The code and commands use R syntax.

The process to generate a nice rendered document from an Rmd file is
known as **knitting**. When you *knit* an Rmd file, various R packages
and programs run behind the scenes. But the process can be broken down
in three main phases: 1) Parsing, 2) Execution, and 3) Rendering.

1)  Parsing: the content of the file is parsed (examined line by line)
    and each component is identified as yaml header, or as markdown
    text, or as R code.

Each component receives a special treatment and formatting.

The most interesting part is in the pieces of text that are R code.
Those are separated and executed if necessary. The commands may be
included in the final document. Also, the output may be included in the
final document. Sometimes, nothing is executed nor included.

Depending on the specified output format (e.g. HTML, pdf, word), all the
components are assembled, and one single document is generated.

### Markdown Syntax

R markdown (`Rmd`) files use
[markdown](https://daringfireball.net/projects/markdown/) as the main
syntax to write content and text.

Markdown is a very lightweight type of [markup
language](https://en.wikipedia.org/wiki/Markup_language), and it is
relatively easy to learn. If you are new to Markdown, please take a look
at the following tutorials:

  - [www.markdowntutorial.com](http://www.markdowntutorial.com)
  - [commonmark.org/help/tutorial](http://commonmark.org/help/tutorial/)
  - [agea.github.io/tutorial.md](http://agea.github.io/tutorial.md/) by
    Andrea Agili

### Rstudio markdown tutorial

RStudio has a basic tutorial about R Markdown files: [Rstudio markdown
tutorial](https://rmarkdown.rstudio.com/lesson-1.html). Take a look at
the following sections:

  - Introduction
  - How It Works
  - Code Chunks
  - Inline Code
  - Markdown Basics
