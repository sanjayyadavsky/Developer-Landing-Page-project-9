# Developer Landing Page project 9

## learning 
when we used **float** property, we have to use **clear** property to clear effect of floating on the oter element 


here the example

``` html
<header>
        <!-- Navigation Bar Starts -->
        <nav>
            <!-- Navigation items Starts -->
            <a class="nav-item">Home</a>
            <a class="nav-item">APIs</a>
            <a class="nav-item">Blogs</a>
            <a class="nav-item">Forums</a>
            <a class="nav-item">LogIn</a>
            <a class="nav-item-active ">Sign Up</a>
        </nav>

        <!-- LOGO -->
        <div >
            <img class="logo" src="./images/Logo.png" >
        </div>
        <!-- Text -->
        <div class="header-text">
            <img src="./images/Rectangle_12.png">
            <h2>
                Lorem ipsum dolor sit amet, <br>consectetur adipiscing elit.
            </h2>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit.
            </p>
        </div>
        <!-- Image -->
        <div>
            <img class="header-image" src="./images/IMAGE HERE.png">
        </div>
    <div class="clearfix"></div>
    </header>

      <!-- Companies -->
    <div class="companies">
        <a href="#" class="company-items">Company One</a>
        <a href="#" class="company-items">Company Two</a>
        <a href="#" class="company-items">Company Three</a>
    </div>
```

and css for this 

```css
.clearfix{
    clear:both;
}
```
### Or even we can give overflaw: hidden ; or overfloaw:auto; but sometime its creat problem while positioning 

```css
header{
    overflow:hidden;
}
```
or we can use alternative method i.e is give clear peoperty to element which is jsut before parent element 
### here is the example 
```css
.companies{
    clear:both;
}
```
Or you can jsut give hight to the property 

```css
header{
    height :500px;
}
```

# learning 
css how to target placeholder 
```html
 <div class="download-email">
                <form>
                    <input placeholder="Enter your email address"/>
                    <button>Download</button>
                  </form>
            </div>
```
css for it
```css
.download-email > form > input::placeholder {
  color: #000;
  opacity: 0.5; /* Firefox */
}
```