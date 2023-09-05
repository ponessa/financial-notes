---
title: Writing your document
permalink: /en/quickstart/writing-your-documents
abstract: >- # this means to ignore newlines until "baseurl:"
  Overview of the components of the markdown document that will become your project documentation.
---

## Overview

Now that you have your site established and the basic structure/table of contents established, it is time to add your documents. To do this:

1. Navigate to the `_docs` directory.

1. Navigate or create the folder as defined in the `docs.yaml`

1. Within that folder create a new file with the name as defined in the `docs.yaml` with the extension `.markdown`.

1. Add the following YAML frontmatter to the top of the file,replacing `title` with the title that you want for the document, and `permalink` and `abstract` with the URL and abstract, respectively, that you want for the document.
```
---
title: Writing your document
permalink: /en/quickstart/writing-your-documents
abstract: >- # this means to ignore newlines until "baseurl:"
  Overview of the components of the markdown document that will become your project documentation.
---
```


## Front matter
Front matter is an area at the top of your Markdown documents that lets you write variables and even content for your pages. It uses YAML, a simple and friendly serialization language, and it works well in combination with Liquid.

Front matter is written with simple YAML variable, using a **key**: **value** notation, with a colon.

Any file that contains a YAML front matter block will be processed by Jekyll as a special file. The front matter must be the first thing in the file and must take the form of valid YAML set between triple-dashed lines. Here is a basic example:

```
---
layout: post
title: Blogging Like a Hacker
---
```

Between these triple-dashed lines, you can set predefined variables (see below for a reference) or even create custom ones of your own. These variables will then be available for you to access using Liquid tags both further down in the file and also in any layouts or includes that the page or post in question relies on.

## Content

Once the front matter has been added, content may be added in either markdown or HTML format. Note that a side **table of content** will be automatically generated based on the headers used within the content.

![Side TOC]({{ site.baseurl }}/assets/images/docs/side-toc.png)