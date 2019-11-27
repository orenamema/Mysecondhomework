# Mysecondhomework

My second homework 



I am going to create a Portfolio using Bootstrap. The first thing that I do is create a HTML file for the about page which will be the main page and 2 others for the Portfolio and the Contact. The objective of this assignment is to make sure that the website is compatible on Mobile devices such as a cell phone or a tablet. Bootstrap gives us the tools to make the website compatible on mobile devices. 



Page #1 About 

To create the About page I’ve used the Navabar for the top container. Using Bootstrap we can use a template on the website which allows us to work faster. In addition of Bootstrap, I will be using style.css to edit the format of the Navbar.



Page #2 Portfolio 





Page #3 Contact



# Homework 2
Using bootstrap to create a Portfolio website 

## Intro

This is a simple Portfolio website that can be accessed at [index.html](index.htlm).
The objective of this assignment is to make sure that the website is compatible on Mobile devices such as a cell phone or a tablet. Bootstrap gives us the tools to make the website compatible on mobile devices. 

![alt text](https://github.com/orenamema/Mysecondhomework/raw/master/images/catch_game.gif)

### Requirements
Some of the rquirements for this page were `bootstrap`, `jquery` and the style.css file generated `style.css`
```html
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
    <script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>
    <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" crossorigin="anonymous"></script>
    <link rel="stylesheet" href="assets/css/style.css"> 
```

## 1 - Clone and build-run the viz server
```Bash
# clone the container
git clone https://github.com/naouss80/qlearncatchd3.git
# access the folder
cd qlearncatchd3/
# build the container
docker build -t viz_server node_container
# run the container
docker run -it -p 80:80 -p 2814:2814 viz_server node viz_server.js debug
```
## 2 - Open the browser
Go to `localhost`
You should see the following


![alt text](https://github.com/naouss80/qlearncatchd3/raw/master/images/start_window.PNG)

## 3 - Get local IP addres and build-run the qlearning app
Get IP adddress for [windows](https://kb.wisc.edu/page.php?id=27309) with `ipconfig /all`.
For Unix systems use `ifconfig`
An example of this can be 10.227.40.281

Open another command line window
```Bash
# assuming one is still in the repository folder 
# build the container qlearncatchd3
docker build -t qlearnin qlearn_container
# run the container
# docker run -it qlearnin python test_catch.py <game> <ip_address> <debug_optional> <node_optional> <count_of_epoch_optional>
docker run -it qlearnin python test_catch.py Catch 10.227.40.281 debug with_node 1000
```

There are 4 games:
* `Catch`: The basket should catch a fruit falling linearly
* `CatchReverse`: The basket should avoid the fruit linearly
* `CatchRandom`: The basket should catch a fruit falling randomly
* `CatchRandomReverse`: The basket should avoid a fruit falling randomly

## 4 - Go back to browser
Go back to the browser and see the training process


![alt text](https://github.com/naouss80/qlearncatchd3/raw/master/images/catch_game.gif)