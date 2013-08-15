Presentify
==========

A simple, self-contained slideshow generator

Presentify is a Python program that reads Markdown files and produces completely self-contained HTML slideshows. It embeds images and fonts so you don't have to worry about flaky Internet connections or missing files. It even works offline! 
Install
=======

    curl https://raw.github.com/tdeitch/presentify/master/presentify.py
    pip install markdown
    chmod +x presentify.py
    ./presentify.py input.md output.html

Markdown file format
====================

- Slides are separated by "---"
- Before the first slide, add a title and author
- Optionally, use `progress: true` to add a progress bar to the slideshow
- Use `bg: `, followed by the local path to a image, the URL of a remote image, or a CSS color to set the page background
- Use `color: ` to set the text color
- Use `class: ` to set optional, slide-level styles
    - `big` makes the font larger
    - `center` centers the text
    - `shout` enlarges and centers the text
