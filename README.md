# EX01 Developing a Simple Webserver
## Date:25.03.2024

## AIM:
To develop a simple webserver to serve html pages.

## DESIGN STEPS:
### Step 1: 
HTML content creation.

### Step 2:
Design of webserver workflow.

### Step 3:
Implementation using Python code.

### Step 4:
Serving the HTML pages.

### Step 5:
Testing the webserver.

## PROGRAM:
```
<!DOCTYPE html>
<html lang="en">
<head>
    {% load static %}
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body{
            margin: 0px;
            padding: 0px;
            box-sizing: border-box;
        }
        .main{
            width: 100%;
        }
        nav{
            width: 100%;
            height: 80px;
            line-height: 80px;
           
            display: flex;
            justify-content: space-between;
        }
        .logo a{
            font-size:39px;
            color: red;
            font-weight: 17px;
            margin-left: 100px;
        }
        a{
            text-decoration: none;
            color: #fff;
            font-size: 18px;
            transition: 0.5s all ease;
        }
        ul{
            margin: 0px;
            margin-right: 100px;
        }
        ul li{
            float: left;
            padding: 0px 15px;
            list-style: none;
        }
        ul li a:hover{
            color: red;
        }
        .header{
            background-image: url("{% static 'images/food.jpg' %}");
            background-position: center;
            background-size: cover;
            background-repeat: no-repeat;
            height: 100vh;
        }
        .content{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    color: #fff;
    text-align: center;
    
}
.content h1{
    font-size: 50px;
}

.content p{
    padding: 0px 70px;
    font-size: 20px;
}

button{
    background: none;
    border: 1px solid #fff;
    color: #fff;
    font-size: 18px;
    padding: 10px 25px;
    border-radius: 6px;
    transition: 0.5s all ease;
}

button:hover{
    background: black;
    color: red;

}

.overlay{
    background: rgba(0,0,0,0.6);
    height: 100vh;
}
    </style>
</head>
<body>
    <div class="main">
        <div class="wrapper">
            <div class="header">
                <nav>
                    <div class="logo">
                        <a href="">AKFood</a>
                    </div>
                    <ul>
                        <li><a href="">HOME</a></li>
                        <li><a href="">ABOUT</a></li>
                        <li><a href="">FOOD</a></li>
                        <li><a href="">BLOG</a></li>
                        <li><a href="">SERVICES</a></li>
                        <li><a href="">CONTACT</a></li>
                    </ul>
                </nav>
                <div class="overlay">
                    <div class="content">
                        <h1>WELCOME TO <br> AKFOOD</h1>
                        <p>Biryani is a flavorful and aromatic dish that originated in the Indian subcontinent, known for its rich blend of spices and tender, marinated meat or vegetables combined with fragrant basmati rice. This beloved dish has many regional variations, each with its unique taste and ingredients, making it a popular choice for special occasions and gatherings.</p>
                        <button>Order Now</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
    
</body>
</html>
```

## OUTPUT:
![alt text](<Screenshot (13).png>)

![alt text](<Screenshot (14).png>)

## RESULT:
The program for implementing simple webserver is executed successfully.
