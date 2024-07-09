# Seaturtle Sites

Sites on Seaturtle browser follow the CARETTA Protocol (Custom Application Rendering Environment and Templating Terminal Application)

## Top Level Domains

There are 10 allowed top level domains:

1. `.turtle`
2. `.seaturtle`
3. `.shell`
4. `.ocean`
5. `.marine`
6. `.waves`
7. `.reef`
8. `.coral`
9. `.sea`
10. `.blue`

## Writing a Website

Websites that run on the CARETTA Protocol use:
1. TurtML (Turtle Markup Language) - Extension: `.turtml`
2. CoralSS (Coral Style Sheets) - Extension: `.coralcss`
3. Python - Extension: `.py`

The entrypoint must be named `home.turtml`

## TurtML
### Syntax
Tags in TurtML follow the following syntax:
```
tag_name(parameters)-- Inner content
tag_name(parameters)-- Inner content --tag_name
```

There are two types of tags, those which require a closing token, and those which do not.

In the example, the former shows the syntax for a tag which does **not** require a closing tag, while the latter shows the syntax for tags which do require closing tags.

#### Comments

Comments follow the following syntax:

```
--- Single line Comment
|-
Multi line Comment (line 1)
Multi line Comment (line 2)
-|
```

#### Metadata

Metadata is added through by the following:

```
--meta(type): value
```

Metadata tags are demarcated by **newlines**

The types of metadata are:
1. `description` - A description of the website, shown by search engines.
    - Aliases: `desc`
2. `name` - The title of the website.
    - Aliases: `title`

Full example:
```
--meta(name): The Seaturtle Project
--meta(description): The homepage of The Seaturtle Project.
```

#### Box
Box tags are equivalents of divs in HTML. They require closing tags.

#### Page
Page tags are similar to boxes. The only difference is that they always cover the viewport.
