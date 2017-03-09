## This is my web page

Pagina destinada para solicitar informacion a instituciones estatales.

 [Second web page](https://luifqui.github.io/GobAbierto/index2)
 
 [access to spreadsheet](https://luifqui.github.io/GobAbierto/accessToSpreadSheet.html)

You can use the [editor on GitHub](https://github.com/luifqui/GobAbierto/edit/master/index.md) to maintain and preview the content for your website in Markdown files.



Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/luifqui/GobAbierto/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
 <script type='text/javascript'>
        var publicSpreadsheetUrl = 'https://docs.google.com/spreadsheets/d/1DuFjsXe9W2T3WliX2yD0aMUK7VP1EdEw07cxs_jveGg/pubhtml';
        var typeoflist = 'ol';
        function init() {

          Tabletop.init({
            key: publicSpreadsheetUrl,
            callback: showInfo,
            simpleSheet: true
          })
        }
        
        function showInfo(data, tabletop) {
          //var list = '<'+typeoflist+'>';
          for (i = 0; i < data.length; i++) {
            //  list += '<li>'+data.length + ' ' + Sheet1.Name.data[i] + '</li>';          
            //}
            //list += '</'+typeoflist+'>';
            //document.getElementById("demo").innerHTML = list;
            //console.log(data);
            var el = document.createElement("option");
            el.textContent = data[i].Institucion;
            el.value = data[i].Direccion;
            select.appendChild(el);
          }
          return true;
        }

</script>