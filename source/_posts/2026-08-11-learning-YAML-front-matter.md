---
title: Learning About YAML Front Matter
tags:
 - blogging 
 - YAML
 - markdown
date: 2026-08-11T23:00:00-04:00
---

### Fun With YAML Front Matter

Here's what my local AI told me about YAML front matter:

~~~yaml
You can include almost any piece of metadata that helps define, categorize, or guide how your content should be displayed or processed by the system reading it (like a static site generator).

Since the function of the front matter is to act as structured data *about* the content rather than the content itself, you can think of it as adding YAML key-value pairs for anything non-narrative.

Here is a comprehensive list of common things you might include:

### 1. Publishing & Timing
These control when and how often the content appears chronologically.

*   **`date:`**: The original creation or publication date (most common).
*   **`pubdate:` / `published:`**: A specific date intended for public viewing, which might be different from the file's actual modification date.
*   **`last_modified:`**: When the content was last substantially edited.

### 2. Categorization & Indexing
These help navigation and filtering on your site.

*   **`tags:`**: A list of keywords (e.g., `["python", "api", "testing"]`).
*   **`categories:`**: Broader groupings, often mutually exclusive to tags (e.g., `"Programming"`).
*   **`series:`**: To link posts that belong to a multi-part tutorial or series.

### 3. SEO & Display Control (For Web Presentation)
These guide search engines and the site's rendering logic.

*   **`slug:`**: A clean, URL-friendly version of the title, often mandatory for creating permalinks (e.g., `my-awesome-post`).
*   **`excerpt:` / `summary:`**: A short summary that should be displayed on an index page without reading the whole article.
*   **`featured_image:`**: To specify a path to an image that should represent the post on index pages.
*   **`canonical:`**: Used for SEO to point search engines to the primary version of a page if multiple URLs exist.

### 4. Per-System Directives (Site Generator Specific)
Some generators have proprietary keys you *must* use to make specific features work:

*   **`layout:`**: Tells the site generator which template file to use for rendering this specific post (e.g., `layout: "video_post"`).
*   **`draft:`**: A boolean flag (`true`/`false`) used to keep posts private until they are ready to go live.
*   **`math_engine:`**: Specific directives needed by LaTeX/MathJax implementations if you embed math equations using specific syntax.

By adding these kinds of structured keys, you turn a simple Markdown file into a self-contained data object that your website software can read and use to build out a complex, functional website.
~~~

Mostly I'm interested in getting the dates right so I can add tehm to the posts.
