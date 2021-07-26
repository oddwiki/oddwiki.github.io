# OddWiki

## What is it?

The [OddWiki](https://oddwiki.github.io/) is an effort to create a fully-sourced encyclopedia about the universe of Oddworld, where unsure fans can visit to make sure their knowledge about anything within it is correct.

## How to Contribute

First fork the repository (you can do this with the Fork button on the top right), you only need to do this once.

1. Navigate to your fork. The URL should be `https://github.com/[YOUR USERNAME]/oddwiki.github.io`.
2. If there is a button called "Pull request" available, press it, select "switch bases" and follow the instructions. You will need to give the pull request a title, but this can be basically anything.
3. Accept the previously created pull request. This has the effect of making your repository up to date.
4. Do your changes. You can change as much stuff as you want.
5. There will once again be a button called "Pull request", follow instructions, give your request a name and then wait until your request is either denied or approved.

## Creating an Article

Every article requires two files: a YAML file, which contains the article's information; and a Markdown file, which feeds that information into the template system to generate the article's page. As an example, let's say we want to create an article about Vykker's Labs. First, we determine the category the article should be in. Since Vykker's Labs is a location, it should be in the Locations category; so we create a new file in `/_data/locations` (note the underscore) called `vykkers-labs.yml` and another file in `/categories/_locations` (again, note the underscore) called `vykkers-labs.md`. If the files already exist, then use those instead; please don't make duplicates! The filenames can ultimately be anything; but they should be short and descriptive and they *must* match. They must also be in lowercase and have no spaces; any spaces in words must be denoted by dashes (\-).

The `vykkers-labs.yml` YAML file is then structured something like this:

```
name: "Vykker's Labs"

quote: "\"Vykker's Labs is an impenetrable fortress.\" - The Almighty Raisin"

summary: |
  Vykker's Labs is a location in [Munch's Oddysee](/games/munchs-oddysee).

appearance: |
  Vykker's Labs is a circular flying fortress.
```

Refer to the corresponding templates in the `_includes` directory (they begin with `info-`) to see all the possible sections in a category. Any section not listed in a YAML file will not be added to the generated page. An important thing to note is that YAML files *do not accept tabs*, so only use spaces or you will end up breaking something. The Markdown file, by comparison, is much simpler:

```
---
layout: index
---
{% include info-locations.md item=site.data.locations.vykkers-labs %}
```

The first part is the template to include, in this case the `info-locations.md` template; and the second part is the YAML file to load which takes the form of `site.data.[CATEGORY].[FILENAME]`. Note that the filename here does not have the `.yml` extension, so make you sure you don't accidentally include it. After you've created these files, you should only ever need to edit the YAML file to update the article in the future. To learn more about how the syntax of these two file types are structured, consult these [YAML](https://learnxinyminutes.com/docs/yaml/) and [Markdown](https://kramdown.gettalong.org/quickref.html) guides.

## OMG I MESSED UP WHAT DO I DO?

In case the version of the wiki you're using is hopelessly broken, you can delete your fork using Setting -> Delete this repository, then forking again; however, this is like a sledgehammer: very powerful, but also very destructive. Please try to fix the problem in a more gentle way if you can. It'll help your blood pressure in the long run.
