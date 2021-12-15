# Accessibility-Refactoring-Client-
semantic Htmls elements were added.
Replaced a lot of unnecessary <dev> tags with appropriate <nav>, <section>, <article>, <footer> tags. 
example:

<code>
<section class="search-engine-optimization">
            <img src="./assets/images/search-engine-optimization.jpg" class="float-left" />
            <h2>Search Engine Optimization</h2>
            <p>
                The dominance of mobile internet use means that users are searching for the right business as they travel, shop, or sit on their couch at home. Search Engine Optimization (SEO) allows you to increase your visibility and find the right customers for your business.
            </p>
        </section>
</code>
 
 <section> was used insead of <dev> because  <section> element is slightly more specific that of a <div>.
--------------------------------------------------------------------------------------------------------------------------------
Minimizing CSS Code lines by Merging three classes with the same properties to one single class. The Old code was using them as IDs when in fact they should've been used as class. 
Example:
 OLD CODE
<code>
.benefit-lead {                             This was the original code.
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-brand {
    margin-bottom: 32px;
    color: #ffffff;
}

.benefit-cost {
    margin-bottom: 32px;
    color: #ffffff;
}
</code>
NEW CODE
</code>                        This is the new code. lbc stands for Lead, Brand, Cost.
.benefit-lbc {                       
    margin-bottom: 32px;
    color: #ffffff;
}
</code>
--------------------------------------------------------------------------------------------------------------------------------