# 🔥Basics

<img src="./assets/images/html.png" alt="html" width="700px">

## ⚡Meta Tags

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <!-- This provides responsive rendering of a website -->
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- To show description related to a website in Search Engines -->
    <meta name="description" content="This is educational content providing website">
    <!-- This is for search engines to cache oursite for keywords typed by a user -->
    <meta name="keywords" content="web development, web design">
    <!-- This tag will allow search engines to not cache our website in their search results -->
    <meta name="robots" content="NOINDEX, NOFOLLOW"> 
    <title>Meta Tags</title>
</head>
<body>
    <h1>Meta Tags</h1>
</body>
</html>
```

## ⚡Typography

```html
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="UTF-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<title>Typography</title>
	</head>
	<body>
		<!-- Headings -->
		<h1>Heading 1</h1>
		<h2>Heading 2</h2>
		<h3>Heading 3</h3>
		<h4>Heading 4</h4>
		<h5>Heading 5</h5>
		<h6>Heading 6</h6>

		<!-- Paragraphs -->
		<p>This is text inside paragraph element.</p>
		<p>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugiat, optio.
            <!-- This is strong tag -->
            <strong>This is bold tag</strong>  
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugiat, optio.
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugiat, optio.
            <!-- This is itallic tag -->
            <em>This is itallic tag</em>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugiat, optio.
            <!-- This is break tag -->
            <br>
            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Fugiat, optio.
		</p>
	</body>
</html>
```

## ⚡Links, Images & attributes

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Links, Images & Attributes</title>
</head>
<body>
    <!-- This is a external link(anchor) tag -->
    <a href="https://gopibabu.live" target="_blank">Gopibabu</a>

    <p>
        <a href="./meta_tags.html">Meta tags inside our project</a>
    </p>
    <p>
        <!-- This is a image tag -->
        <img src="https://source.unsplash.com/user/erondu/1600x900" alt="learning" width="300">
    </p>
</body>
</html>
```

## ⚡Lists & Tables

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lists & Tables</title>
</head>
<body>
    <!-- unordered lists -->
    <ul style="list-style:square;">
        <li>Unordered list item 1</li>
        <li>Unordered list item 2</li>
        <li>Unordered list item 3</li>
    </ul>

    <!-- ordered lists -->
    <ol type="A">
        <li>ordered list item 1</li>
        <li>ordered list item 2</li>
        <li>ordered list item 3</li>
    </ol>

    <!-- nested lists -->
    <ul style="list-style:square;">
        <li>Unordered list item 1</li>
        <li>Unordered list item 2</li>
        <li>
            Unordered list item 3
            <ol type="A">
                <li>ordered list item 1</li>
                <li>ordered list item 2</li>
                <li>ordered list item 3</li>
            </ol>
        </li>
    </ul>

    <!-- tables -->
    <table style="border: 1px solid red;">
        <thead>
            <tr>
                <th>Table Heading 1</th>
                <th>Table Heading 1</th>
            </tr>
        </thead>
        <tbody>
            <tr>
               <td>data 1-1</td>
               <td>data 1-2</td> 
            </tr>
            <tr>
                <td>data 2-1</td>
                <td>data 2-2</td> 
             </tr>
        </tbody>
    </table>
</body>
</html>
```

## ⚡Forms & Input

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Forms & Input</title>
</head>
<body>
    <form action="#" method="get">
        <div>
            <label for="name">Name:</label><br>
            <input type="text" name="name" id="name">
        </div>
        <div>
            <label for="email">Email:</label><br>
            <input type="email" name="email" id="email">
        </div>
        <div>
            <label for="message">Message:</label><br>
            <textarea name="message" id="message" cols="50", rows="5"></textarea>
        </div>
        <div>
            <label for="sex">Sex:</label><br>
            <select name="sex" id="sex">
                <option>Select</option>
                <option>Male</option>
                <option>Female</option>
            </select>
        </div>
        <div>
            <label for="Age">Age:</label><br>
            <input type="number" name="age" id="age">
        </div>
        <div>
            <label for="birth_date">Birth Date:</label><br>
            <input type="date" name="birth_date" id="birth_date">
        </div>
        <div>
            <label for="membership">Membership:</label><br>
            Basic
            <input type="radio" name="membership" id="membership" value="Basic"><br>
            Premium
            <input type="radio" name="membership" id="membership" value="Premium"><br>
            Platinum
            <input type="radio" name="membership" id="membership" value="Platimun">
        </div>
        <div>
            <label for="preferences">Preferences:</label><br>
            Bus
            <input type="checkbox" name="preferences" id="preferences" value="Bus"><br>
            Train
            <input type="checkbox" name="preferences" id="preferences" value="Train"><br>
            Plane
            <input type="checkbox" name="preferences" id="preferences" value="Plane">
        </div>
        <input type="submit" value="Submit">
        <button type="reset">Reset</button>
    </form>
</body>
</html>
```

## ⚡Block & Inline Elements

```html

<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="UTF-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<title>Block & Inline Elements</title>
	</head>
	<body>
		<!-- Block level Elements -->
		<p>
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore nisi
			facere iure harum, vitae possimus voluptates sint deleniti dignissimos
			dolores.
        </p>

        <div id="main-header">
            <h1>My Website</h1>
            <p class="main-para">A site about me</p>
        </div>

        <!-- Inline Elements -->
        <a href="#">Google</a><a href="#">Facebok</a>
        <span>Span 1</span><span>Span 2</span>
        <img src="https://source.unsplash.com/user/erondu/100x100" alt="..">
        <img src="https://source.unsplash.com/user/alexmotoc/100x100" alt="..">
	</body>
</html>

```

## ⚡HTMl Entities

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Entities</title>
</head>
<body>
    <!-- Non Breaking Space -->
    <p>Hello, My name is &nbsp; &nbsp; &nbsp; Gopibabu</p>

    <!-- Greater than & Less than -->
    <p>5 &gt; 2</p>
    <p>1 &lt; 2</p>

    <!-- Copyright -->
    <p>&copy;</p>
    <p>&reg;</p>

    <!-- Currency -->
    <p>&cent;</p>
    <p>&pound;</p>
    <p>&yen;</p>
    <p>&euro;</p>

    <!-- Suits -->
    <p>&spades;</p>
    <p>&diams;</p>
    <p>&clubs;</p>
    <p>&hearts;</p>

    <!-- Computer Code -->
    <code>
        &lt;?php
        echo phpinfo();
    </code>
</body>
</html>
```

## ⚡HTML5 Semantic Tags

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML5 Semantic Tags</title>
</head>
<body>
    <header>
        <p>This is  head section</p>
    </header>
    <nav>
        <p>This is navbar section</p>
    </nav>
    <main>
        <p>This is main content area</p>
        <section>
            <p>This is a section inside main content area</p>
            <article>
                <p>This is article section inside a section in main content area</p>
            </article>
        </section>
        <aside>
            <p>This is a a sidebar section inside main content area</p>
        </aside>
    </main>
    <footer>
        <p>This is  footer section</p>
    </footer>
    <p style="color: blueviolet;">Contents are aligned properly using CSS</p>
</body>
</html>
```
