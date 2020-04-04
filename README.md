# oddwiki.github.io

## How to contribute

First fork the repository (you can do this with the Fork button on the top right), you only need to do this once.

1. Navigate to your fork. The URL should be `https://github.com/[YOUR USERNAME]/oddwiki.github.io`.
2. If there is a button called "Pull request" available, press it, select "switch bases" and follow the instructions. You will need to give the pull request a title, but this can be basically anything.
3. Accept the previously created pull request. This has the effect of making your repository up to date.
4. Do your changes. You can change as much stuff as you want.
5. There will once again be a button called "Pull request", follow instructions, give your request a name and then wait until your request is either denied or approved.

## File naming requirements

First, locate the category you want to place your file in. Let's say, we want to create an article about Vykkers Labs. We should go to `_locations` and inside there create a new file (unless it already exists, please don't make duplicates!) called `vykkerslabs.md`, the file name can be anything, but it should be short, descriptive, all lowercase, with no spaces allowed (though if you really want to, you can add \_-s), and should end with ".md".

The content should be formatted using Markdown ([guide](https://kramdown.gettalong.org/quickref.html)). Every file must begin with the following:

```
---
title: "[Title of the page]"
---

```

So in the previous example, it would be

```
---
title: "Vykkers Labs"
---

Vykkers Labs is a location in Munch's Oddysee. . .
```

## OMG I MESSED UP WHAT DO I DO?

In case the version you're using is hopelessly broken, you can delete your fork using Setting -> Delete this repository, then forking again. However, this is like a sledgehammer, very powerful, but also very destructive. Please try to fix the problem in a more gentle way if you can. It'll help your blood pressure in the long run.
