---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Organizing a project knowledge base"
subtitle: ""
summary: ""
authors: []
tags: []
categories: [professional]
date: 2022-04-29
lastmod: 2022-04-29
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
#image:
#  caption: "Ladybug on fennel blossom"
#  focal_point: "Smart"
#  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---
I have found myself running up against the practical limits of individual notebooks and email archives full of meeting minutes and scattered notes about papers and other materials that I've read, despite those notebooks at least being searchable. When I need to revisit a justification for making a particular project decision or to find data on related work, I often end up re-reading papers and many meeting minutes to collect the relevant tidbits. I can even end up looking for the same information repeatedly. Having individual notebooks maintained by different team members can also slow down the process of finding all relevant information for a given topic and reaching consensus. Onboarding new team members is made more cumbersome by needing to forward siloed information, too. So, it's worthwhile to be deliberate about choosing how to effectively maintain a project knowledge base.

There are innumerable possible tools for maintaining knowledge bases for project teams, some of which are hiding in plain sight, and selecting one that minimizes friction overall has required a substantial amount of experimentation and reading to balance tradeoffs. In this post, I want to document those considerations that have led me to conclude for now that [GitHub wikis](https://docs.github.com/en/communities/documenting-your-project-with-wikis) in [Asciidoc](https://asciidoctor.org/) mode may be a good option for the sorts of projects that I'm involved in. Of course, the considerations may be different for other teams and projects.

The main aspects that I considered are:
1. Enabling participation without requiring specialized tools to be installed
2. Integration with existing services that we already use in the project
3. Searchability
4. Navigability
5. Fine-grained cross referencing
6. Bibliography support
7. Diagramming support
8. Maintaining a logical history
9. Data portability
10. Support for a range of screen sizes

I'll cover the details of each of these below.

## Enabling participation without requiring specialized tools to be installed

Requiring specialized tools can be a barrier to participation for obvious reasons.

GitHub wikis can be viewed and edited directly in the browser without requiring any additional tools.

Admittedly, the GitHub graphical wiki editor is not a full WYSIWYG. Editing is only supported in text/code mode, and a separate preview tab is used to show the formatting. However, the formatting notation is human-readable so as to make editing the underlying code for each page more intuitive.

GitHub wikis are managed as human-readable and -editable files in a git repository, so team members also have the option of cloning that repository and editing it outside of the online tools.

## Integration with existing services that we already use in the project

This is closely related to the prior consideration. Just as requiring specialized tools can be a barrier to participation, so can requiring team members to sign up for a new service. When GitHub is already used for managing source code, that eliminates what would have otherwise been a hurdle to using GitHub wikis.

Another advantage is that this integrates access control settings as well.

## Searchability

Surprisingly, this is something that can't be taken for granted, even in modern tools. Since GitHub wikis are viewable in web browsers, browser search tools automatically apply. The main GitHub search function also covers wiki content. It's necessary to manually click the wiki tab in search results for those instances to be displayed.

Furthermore, since the files backing the wiki are human-readable and can be cloned, the full array of tools for searching text files also become applicable.

## Navigability

This is related to but also distinct from searchability. This is the ability to view and browse the structure of the knowledgebase. Essentially, this boils down to the tool providing an automatically generated table of contents.

## Fine-grained cross referencing

It is important to be able to cross reference pages in a knowledge base. Furthermore, certain pages can become quite lengthy, so it's important to even be able to link to particular elements within those pages.

Cross-referencing in GitHub wikis works a little differently than it does for Asciidoc files outside GitHub wikis. For reference, the default Asciidoc approach is described [here](https://docs.asciidoctor.org/asciidoc/latest/macros/inter-document-xref/#navigating-between-source-files). However, in GitHub wikis, using that syntax links to the raw text of the specified portion of the document.

To link to the formatted text, ordinary link syntax can be used. For example, to link to a heading "Heading 1" in a page titled "Cross ref page", the following syntax works:
```
link:Cross-ref-page#heading-1[Heading 1]
```
Spaces are replaced by dashes, headings are converted to lowercase, and text for the link is inserted in the square brackets.

Intra-document cross-references can also be [created](https://docs.asciidoctor.org/asciidoc/latest/macros/xref/#internal-cross-references).

## Bibliography support

Bibliographies are crucial in scientific projects. Asciidoc supports them [directly](https://docs.asciidoctor.org/asciidoc/latest/sections/bibliography/).

## Diagramming support

This is an area of strength for alternative tools that allow creating diagrams using a graphical tool directly inline in the document. GitHub wikis do not yet support that. Asciidoc supports a variety of [types of diagrams](https://docs.asciidoctor.org/diagram-extension/latest/) that can be generated from text descriptions, but that is more tedious that graphically editing diagrams in many cases, and I am unsure of the extent of GitHub's current support (if any) for those diagrams.

However, at least GitHub supports pasting images into Asciidoc wiki pages. That said, they currently insert Markdown syntax referencing the pasted pictures, even when Asciidoc mode is selected. I reported this bug to GitHub, so hopefully it will be resolved eventually. Meanwhile, the image links need to be manually converted into [Asciidoc syntax](https://docs.asciidoctor.org/asciidoc/latest/syntax-quick-reference/#images).

## Maintaining a logical history

It is important to know the sources for each piece of information. For information derived from other linkable documents, that is the role of the bibliography. However, for information recorded during meetings, there is no previous document that can be linked. One approach would be to define bibliography entries specifying the meeting information, but that could become tedious.

A relevant advantage of maintaining a wiki in git is that it allows grouping changes due to a meeting into a combined commit with a log message specifying the meeting information. Git allows looking up how any piece of content in a repository has been modified over time and viewing the associated commit log messages. However, this currently seems to require using offline tools directly on the underlying git repository. Conversely, it is also possible to quickly view in the repository history all of the changes that were introduced as a result of a specified meeting.

## Data portability

Asciidoc is a widely supported data format that is both human- and machine-readable.

## Support for a range of screen sizes

Team members may use a variety of screen sizes to view content. GitHub wikis automatically adjust the content formatting and layout to accommodate different screen sizes.
