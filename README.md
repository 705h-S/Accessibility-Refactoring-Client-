# Horiseon refactoring code
 Refactored Horiseon's site codebase so that it complies with accessibility standards and is optimized for search engines all with out changing the websites UI. 

---

## Built With

* [HTML](https://developer.mozilla.org/en-US/docs/Web/HTML)
* [CSS](https://developer.mozilla.org/en-US/docs/Web/CSS)
---
## Deployed Link

* [Horiseon]( https://705h-s.github.io/Alpha-Horisen-Refactor/
)

![Webpage](images/WEBPAGE.png)

---

## Refactoring 
First initial look at the HTML source code I didn't find a lot of semantic HTML elements. 
* [Semantic HTML Elements](https://www.w3schools.com/html/html5_semantic_elements.asp)
<br>

For example in the original code  `<Div>`  tags were used instead of  `<footer>`  tags. 
<br>
-**Original Code**-
<br>

```html
<div class="footer">
        <h2>Made with ❤️️ by Horiseon</h2>
        <p>
            &copy; 2019 Horiseon Social Solution Services, Inc.
        </p>
    </div>
```
<br>

By changing the tags it allows the site to be more accessible. It also removes the need to use a `<class="footer">` tag. In CSS they can use a element selector instead of a class selector.

-**New Code**-

<br>

```HTML
<footer>
        <h4>Made with ❤️️ by Horiseon</h4>
        <p>
            &copy; 2019 Horiseon Social Solution Services, Inc.
        </p>
    </footer>
```
<br>

 > Note that the heading attributes were also changed to fall in a sequential order. 
<br>

Another change was made to the `<title>` of sourcecode. 
In the original code it was stated as `<title>website</title>` and for it to be optimized in search engines it was changed to `<title>Horiseon</title>`.

![title](images/Title.png)

---
## Issue and resolvement 
An issue within the site was that when user clicked on one of the nav links it wouldn't take them directly to the corresponding topic in the site itself.

This was resolved by revisiting the index.html and looking over the code that's conntected to the nav links. Upon insepection I found an `<ID="">` was missing. By adding the missing code nav links now work and issue was resolved. 


---
## License
Site and Company owned by respective 
© 2019 Horiseon Social Solution Services, Inc.

---
##### Refactoring done by Joshua Meza
[GitHub](https://github.com/705h-S)
