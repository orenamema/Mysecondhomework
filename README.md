# Homework 2
Using bootstrap to create a Portfolio website 

## Intro

This is a simple Portfolio website that can be accessed at [index.html](index.htlm).
The objective of this assignment is to make sure that the website is compatible on Mobile devices such as a cell phone or a tablet. Bootstrap gives us the tools to make the website compatible on mobile devices. 

There are 3 pages:
* `index.html`: My description
* `portfolio.html`: The portfolio I will build
* `contact.html`: How to get in touch with me

![alt text](https://github.com/orenamema/Mysecondhomework/raw/master/assets/images/demoGIf.gif)

### Requirements
Some of the requirements for this page were `bootstrap`, `jquery` and the css file that I created `style.css`

```html
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" crossorigin="anonymous"></script>
<link rel="stylesheet" href="assets/css/style.css"> 
```

## Website

All pages have `navbars` and `footers`, they also use `containers` and follow the grid framework from bootstrap
```html
<nav class="navbar navbar-default bg-white">
    <div class="container" id="top-container">
```

### About 

The about page contains a picture and many other items that are formated as requested instructions
```html
<img id="orenPic" src="assets/images/oren-picture.png" class="rounded float-left" alt="orenPic">
```
![alt text](https://github.com/orenamema/Mysecondhomework/raw/master/assets/images/about.png)

### Portfolio 
On the portfolio page, we use `cards`, `columns` and `rows`
```html
<div class="row">
    <div class="col-sm-6">
        <div id="nycCard" class="card" style="width: 18rem;">
            <img src="assets/images/newyork.jpg" class="card-img-top" alt="...">
```
![alt text](https://github.com/orenamema/Mysecondhomework/raw/master/assets/images/portfolio.png)

### Contact
The contact page we used `form-group`
```html
<div class="form-group">
    <label for="inputName">Name</label>
```
![alt text](https://github.com/orenamema/Mysecondhomework/raw/master/assets/images/contact.png)
