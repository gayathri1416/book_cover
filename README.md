# Ex.06 Book Front Cover Page Design
# Date:23.09.2025
# AIM:
To design a book front cover page using HTML and CSS.

# DESIGN STEPS:
## Step 1:
Create a Django Admin project.

## Step 2:
Create an app in the Django interface.

## Step 3:
Create a folder named 'static' in the app folder.

## Step 4:
Create a new HTML file in the static folder.

## Step 5:
Write the HTML code with relevant CSS properties.

## Step 6:
Choose the appropriate style and color scheme.

## Step 7:
Insert the images in their appropriate places.

## Step 8:
Publish the website in the LocalHost.

# PROGRAM:
```
    views.py :

    from django.shortcuts import render
def p8(request):
    return render(request,'book.html')

urls.py:

from django.contrib import admin
from django.urls import path
from bookapp import views

urlpatterns = [
    path('admin/', admin.site.urls),
    path('',views.p8,name="cover"),
]

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Book Cover</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: #111;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .book-cover {
      position: relative;
      width: 400px;
      height: 600px;
      border-radius: 15px;
      overflow: hidden;
      box-shadow: 0 8px 20px rgba(0,0,0,0.6);
      font-family: Arial, Helvetica, sans-serif;
      color: white;
    }

    .book-cover >img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }

    .overlay {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: rgba(0,0,0,0.5);
    }

    .insight {
      position: absolute;
      top: 20px;
      left: 20px;
      font-size: 18px;
      font-weight: bold;
      letter-spacing: 2px;
    }

    .Content {
      position: absolute;
      top: 40%;
      left: 50%;
      transform: translate(-50%, -50%);
      text-align: center;
    }

    .title {
      font-size: 38px;
      margin: 0;
    }

    .subtile {
      font-size: 20px;
      margin: 10px 0 0 0;
      font-weight: 300;
    }

    .author-details {
      position: absolute;
      bottom: 20px;
      right: 20px;
      text-align: right;
    }

    .author-pic {
      width: 30x ;   
      height: 30px ;
      border-radius: 50%;
      object-fit: cover;
      margin-bottom: 5px;
      border: 1px solid white;
    }

    .author-name {
      margin: 0;
      font-size: 14px;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <div class="book-cover">
    <img src="bg.jpg"alt="Book Background">
    <div class="overlay"></div>

    <div class="insight">FUTURE WORLD</div>

    <div class="Content">
      <h1 class="title">AI TOOLS</h1>
      <h2 class="subtile">INTRODUCTION OF AI TOOLS</h2>
    </div>

    <div class="author-details">
      <img class="author-pic" src="author.jpg"Author Photo">
      <h5 class="author-name">By GAYATHRI.C</h5>
    </div>
  </div>
</body>
</html>

```
# OUTPUT:
![alt text](<Screenshot 2025-10-05 110945.png>)
# RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
