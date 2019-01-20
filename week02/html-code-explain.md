![TO LOGO](../images/to-logo.jpg)

# COMP.5209 - Interface Analysis and Design

## Week 02 - Lesson 02 (3 hours)
### Prepared by: Jeffrey Kranenburg

# HTML Reference material

## Intro to HTML syntax

* General Layout of document
* Head Tag
* Div and span tags (block and inline)
* Heading Tags
* Images
* Links
* Tables

# General Layout of document

Talk about the follow parts and tags

* `head` `body` `html` `doctype`
* Semantic Tags `header` `footer` `nav` `section` `article` 
* HTML 5 no longer require to have a `/` (forward slash) when closing a self closing tag
* Write all your code in lowercase - program language are there to match english grammar
* Explain how a tag works and what attributes are

# Head Tag

In this tag we place all the information for the website that is needed for search engines, device optimazation and titles.

There are a lot of these tags and not all of them are required for every project.

Some tags however are a must:

| Tag | Description | 
| --- | --- |
|`<meta charset="utf-8" />` | Sets the character encoding |
| `<meta name="viewport" content="initial-scale=1, width=device-width, height=device-height, viewport-fit=cover">` | Stop the content from scaling on a (mobile) device |
| `<title>YOUR TITLE</title>` | Title that appears in the tab bar of a browser |
| `<link rel="stylesheet" href="style.css">` | Your external CSS file |

The following tags are strongly recommended

| Tag | Description | 
| --- | --- |
| `<meta name="description" content="My website is about this....">` 
| A sentence that describes your website |
| `<meta name="keywords" content="some, keywords, to say, what this website, is about" >` 
| Keywords for the search engine that help people find your website (SEO) |
| `<link rel="icon" type="image/png" sizes="16x16" href="static/icons_launch/16x16.png" />` 
| A favicon is the little icon you see next to the url in the address bar |

(Note that keywords can be group if we want to pair up search combinations)

# Div and span tags (block and inline)

Difference between block and inline tags. 
* Block tags always start on a new line
* Inline tags can be placed side by side
* Inline-Block is an option for block tags to be placed side-by-side
* Styling with block tags vs styling by inline tags

# Heading Tags

H1 - H6

* H1 is for page titles
* H2 and smaller is for section titles
* Typography is important in a website, we will spend more time on it later in the course.

# Images

* Add an image using the `<img>` tag
* Always use the `alt` attribute
* This is an example of a self closing tag, since you point to the content inside of an attribute.

```
    <img src="../images/to-logo.jpg" alt="TO Logo">
          |______________________|    |_________|
          Location of image            Name of image
          using relative path          for screen readers
```

# Links

Links are used to navigate to other pages. This is done using anchor tags.

* An anchor tag is setup using the letter a (`<a href="..."`>)
* The a tag must be accomponied by an `href` attribute which holds the place where we go once a person clicks on it.
* For the content of the tag we show the use what they are going click on

```
    <a href="https://google.com">Go to Google</a>
         |_________________|      |________|
          location of place        what the user sees
```

# Tables

Tables are argbuably one of the hardest things to put the together since they are a collection of tags.
* Tables are a collection of rows and columns.
* Inside of a row (using the `tr` tag) we create data cells using the `td` tag.
* We can also define heading cells using the `th` tag instead of a `td` tag.
* Using the `thead` and `tbody` we can define where one area starts and another begins. This help when for when we use CSS to style the table.
* Note in old versions of HTML and for backwards compatibilty HTML5 allows for some styling atrributes, but you should now do all styling inside of CSS>

* Below you will see an example for an HTML Table.
* Note that some columns we might want to centre the data for, but we will get to that later. For now, just focus on the structure.

```
<table>
    <thead>
        <tr>
            <th>
                Month
            </th>
            <th>
                Number of days
            </th>
            <th>
                First Day 2019
            </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                January
            </td>
            <td>
                31
            </td>
            <td>
                Tuesday
            </td>
        </tr>
        <tr>
            <td>
                February
            </td>
            <td>
                28
            </td>
            <td>
                Friday
            </td>
        </tr>
        <tr>
            <td>
                March
            </td>
            <td>
                31
            </td>
            <td>
                Friday
            </td>
        </tr>
    </tbody>
</table>
```

This will look like:

<table>
    <thead>
        <tr>
            <th>
                Month
            </th>
            <th>
                Number of days
            </th>
            <th>
                First Day 2019
            </th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                January
            </td>
            <td>
                31
            </td>
            <td>
                Tuesday
            </td>
        </tr>
        <tr>
            <td>
                February
            </td>
            <td>
                28
            </td>
            <td>
                Friday
            </td>
        </tr>
        <tr>
            <td>
                March
            </td>
            <td>
                31
            </td>
            <td>
                Friday
            </td>
        </tr>
    </tbody>
</table>