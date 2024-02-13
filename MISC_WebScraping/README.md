# Web-Scraping

Overall goal here is to introduce students to html (and, to a lesser extent, css) and to illustrate the use of `BeautifulSoup` to parse it.

Materials:
- [Google Slides: Webscraping](https://docs.google.com/presentation/d/1gYjgl2ztoMf8FI81ebShd1-A8mbjxYin65xT2Cl3P8o/edit)
- [Jupyter Notebook: Webscraping](webscraping.ipynb)

## Learning Goals

- Parse HTML and CSS elements in webpages
- Use `requests` and `BeautifulSoup` to get and process webpage contents
- Use ethics when scraping websites

## Lesson Plan

### Intro (5 Mins)

Webscraping as another way to get data. Webscraping as not first resort! Often better to use flat files or APIs if they're available.

### Webscraping Slides (10 Mins)

### Basic Terminology / Tags (10 Mins)

Go through a few simple types of tags (p, a, head, body), as well as how the nested structure leads to "parent", "child", and "sibling" nomenclature.

### Write some html (10 Mins)

Use the webpage (link in ntbk) to see html rendered in real time. Nice also at this point to show the advantages of using VS Code to write html.

### Basic Return Objects of BeautifulSoup (15 Mins)

Useful to compare this hierarchical structure to JSON, which students will have just learned about. Look at the children of a tag, children of those children etc. We can keep "diving" to get as deep into the code as we need.

### More Sophisticated Pages (10 Mins)

The table is a nice way of showing both the deep structure of some webpages and the utility of pulling out the data, putting into `pandas` etc.

## Tips

- For the webpage creation, it's nice to use [this site](https://htmledit.squarefree.com/) to render sample html code. When I create the html file, I'll edit it in VS Code. VS Code is nice since it will automatically generate closing tags when I create opening tags (if the file has an .html extension). (Keep it simple: A couple headers. Maybe a list.)
