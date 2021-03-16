[<<< Previous](pedagogy.md) | [Next >>>](review.md)   

# Style Guide

# Module Checklist
 
Every module in the curriculum should have these elements:

- A dedicated repository on GitHub
- A README.md file.
- Four elements present in the README.md file: 
  - a `h1` level heading with the name of the tutorial
  - a short paragraph with an accessible description of the technique
  - a short paragraph with the goals or outcomes of the workshop
  - a table of contents with links to the topics in the tutorial
- An introductory page describing the technique or technology in more detail, ideally also explaining the purpose or value of the approach
- A page or pages with installation or setup instructions
- A page or set of pages for each major concept or milestone in the tutorial.
- "<<< Previous" and "Next >>>" buttons on each page that indicate the path a reader will take through the tutorial.
- Code segments should be denoted using the markdown syntax for code and interspersed with explanations. Large blocks of unexplained code should be avoided, but if they're necessary link to a raw text file or Jupyter notebook within the explanatory text. 
- The tutorial should ideally build incrementally toward a larger goal or project and produce some kind of product, whether a visualization, webpage, repository, analysis, app, or draft writing/proposal. The tutorial should be iterative and purposeful—don't just cover material to cover material.
- When possible, prefer techniques or approaches from other DHRI tutorials.
- Everything substantially covered verbally or through slides in a tutorial should appear in the markdown version. Someone not present at the event or who can not hear or see the materials presented should still, in theory, be able to follow based on the materials provided in the markdown tutorial.
- If many topics or headings are included in the tutorial (more than 6), the markdown files other than the README.md should be placed in a folder within the repository labelled `sections` or similar and linked from there. (Having too many files in the files section on GitHub looks messy and is visually overwhelming.)
- If applicable, provide a `resources` section with links to sources, books, tools, or other tutorials at the end of your markdown tutorial.
- While you have the option to create tutorials under your own name on GitHub, when finished or when you reach a major milestone with your tutorial, fork it to the [Research Services & Workshops](https://github.com/orgs/SouthernMethodistUniversity/teams/research-services-and-workshops) account on GitHub for reference by future instructors.


# GitHub Formatting 
Formatting should be as follows:
Separate paragraphs with a blank line.
Place blank lines between elements whenever possible. For example, put a blank line between a heading and a paragraph, and between a paragraph and an image link.
Use headings consistently, and use them only to denote new sections. For example, do not use headings for emphasis.
Use other markdown elements for their intended purpose. Use lists for lists and emphasis for emphasis. For example, do not use emphasis in place of a heading.
Unless a raw URL is part of the tutorial, don't leave raw URLs in your document. Incorporate the link into the flow of your prose.
If code segments are short, indicate them by indenting. If they're longer, use the ````` syntax.
When introducing new commands or code, put them on a new line so they stand out from the rest of the text.
When including images, don't leave the alt text segment [] blank. Fill it in with information that would be useful if the image could not be seen or rendered.
Is coding consistent throughout module?
First header is H1, secondary headers H2, etc. (H1 only used at top of page, H2 used to break sections into chunks, H3 only used if necessary within sections that already have an H2. Compare to outline format:
H1 (title of page)
H2 (first section)
H3 (point 1)
H3 (point 2)
H3 (point 3)
H2 (second section) with no H3 titles necessary
H2 (third section)
Are there any extraneous Markdown tags due to errors in coding? (hashtags, dashes, etc.)
If many topics or headings are included in the tutorial (more than 6), the markdown files other than the README.md should be placed in a folder within the repository labelled sections or similar and linked from there. (Having too many files in the files section on GitHub looks messy and is visually overwhelming.)
While you have the option to create tutorials under your own name on GitHub, when finished or when you reach a major milestone with your tutorial, fork it to the DHRI account on GitHub for reference by future instructors.
Do we want to include the contribution information in the style guide?
Hyperlinks: 
Do all modules have working Previous/Next links at the top and bottom of each page?
Have all links embedded in the module been tested and updated if necessary, or removed if necessary?

## Grammar
Check all spelling and punctuation throughout. 
All bulleted lists should end in some type of end mark (period, question mark, etc.).
Read through all content to make sure sections or content is not duplicated or repetitive, or that there are not disruptive jumps from one topic to another without explanation.

## Markdown Guidelines

### On Markdown

Markdown is a plain text markup format that is easy to read for both computers and humans. This is in contrast to, for example, HTML, which in its unrendered form is not enjoyable for humans to read. Compare the same document in HTML and markdown:

HTML:

```html
<h1>My Book Report</h1>
  <p><i>Persuasion</i> is an <strong>excellent</strong> book that I highly recommend for three reasons:</p>
  <ul>
	<li>It's a comeback story.</li>
	<li>It has a catchy title.</li>
	<li>It's written by Jane Austen.</li>
  </ul>
  <p>You can buy the book <a href="http://www.bookmonopoly.com/persuasion">here.</a></p>
```

Markdown:

```markdown
# My Book Report

*Persuasion* is an **excellent** book that I highly recommend for three reasons:

- It's a comeback story.
- It has a catchy title.
- It's written by Jane Austen.

You can buy the book [here](http://www.bookmonopoly.com/persuasion).
```

When rendered by a browser, both of these documents look identical. However, the markdown document is considerably easier to read in its source form. While HTML is optimized to be readable by the computer, markdown is more balanced between the human and the machine.

### Why Use Markdown?

We use markdown for tutorials for a number of reasons:

- It's exportable to other formats, such as HTML, PDF, and GitBook.
- It can be kept under version control—with Git, for example.
- It's rendered automatically on GitHub.
- It can be read locally with a text editor.
- As plain text, it's maintainable.
- It's easy to embed code and images.
- It plays well with the tools we teach at the DRI.

Many of markdown's advantages come from the fact that it's plain text. Tools that work well with code, such as version control, editors, and grep, also work well with markdown.

### Markdown Formatting

Most formatting guidelines here are designed to make markdown source files more readable. Others are designed to preserve semantics, which allow markdown to be rendered the same in different contexts.

1. Separate paragraphs with a blank line.
2. Place blank lines between elements whenever possible. For example, put a blank line between a heading and a paragraph, and between a paragraph and an image link.
3. Use headings consistently, and use them only to denote new sections. For example, do not use headings for emphasis.
4. Use other markdown elements for their intended purpose. Use lists for lists and emphasis for emphasis. For example, do not use emphasis in place of a heading.
5. Unless a raw URL is part of the tutorial, don't leave raw URLs in your document. Incorporate the link into the flow of your prose.
6. If code segments are short, indicate them by indenting. If they're longer, use the ````` syntax.
7. When introducing new commands or code, put them on a new line so they stand out from the rest of the text.
8. When including images, don't leave the alt text segment `[]` blank. Fill it in with information that would be useful if the image could not be seen or rendered.

## Attribution

## Free and Open Source Code

In general, it's not necessary to provide in-line citations in the materials for a technical workshop unless you're using someone else's exact prose or you're replicating a significant, non-trivial section of code. For example, code segments found on Stack Overflow do not need to be cited unless you think it's pedagogically helpful. However, if you build your session around replicating a significant portion of a particular application, you must consider the license under which that software is released and consider providing attribution, even if attribution is not required under the terms of the license. In general, free and open source code licenses do not require attribution, but using a large portion of the code may require replicating the license. Check a summary of the terms of the license (or the license itself, if you're feeling adventurous) if you decide to replicate a significant portion of an open-source project in your session.

## Citation practices for workshops

Many of the workshops in this curriculum were created by multiple creators. This makes the process of attributing of each other a bit messy. An interested person can see the precise details what was done and by whom in what order in the GitHub commit log. However, we also realize that folks reading this curriculum may not be Git-literate (yet!) or may access this curriculum as a .PDF or a hard copy document offline. Thus, it is also important to attribute the labor of individual contributors in written form at the beginning of each workshop and every other section of this curriculum. 

Currently, the workshops include two forms of attribution: "Session leader: ..." and "Based on previous work by ..."—the former indicates the person who will be the lead teacher of the workshop during the Summer 2020 DHRI session, and the latter indicates who worked on the content of the workshop. We recognize that both are significant attributions, but that the latter is especially important in terms of citation politics, particularly for students and junior scholars. So, despite its redundancy, we listed a contributors name twice if they both are leading the workshop in June 2018 and if they created or significantly contributed to or revised the workshop's content. It is also of note that various contributors edited the content of each others' workshops.  

In regards to citing other academics, this curriculum aims to follow commonly held academic citational practices, in which direct quotations are formatted and cited as such, and when another scholar's ideas or concepts are referenced, a citation is also included. In general, the following citational information is provided: the author name(s), publication title, and publication date, and a hyperlink to the source, if applicable and within copyright.  



[<<< Previous](pedagogy.md) | [Next >>>](review.md)   