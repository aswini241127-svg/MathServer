# Ex.05 Design a Website for Server Side Processing
## Date:

## AIM:
 To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side. 


## FORMULA:
P = I<sup>2</sup>R
<br> P --> Power (in watts)
<br> I --> Intensity
<br> R --> Resistance

## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Create python programs for views and urls to perform server side processing.

### Step 5:
Create a HTML file to implement form based input and output.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```
math.html

<!DOCTYPE html>
<html>
  <head>
    <title>Area of a Rectangle</title>
    <style>
      body {
        background-color: #48a5f0e2;
        font-family: Arial, sans-serif;
      }

      .box {
        width: 500px;
        margin: 100px auto;
        background-color: #4c5cd6eb;
        padding: 30px;
        border: 5px line rgb(50, 191, 206);
        color: white;
        text-align: center;
      }

      h1 {
        color: pink;
      }

      input {
        width: 200px;
        padding: 5px;
        margin: 8px;
      }

      button {
        padding: 5px 15px;
        margin-top: 10px;
      }
    </style>
  </head>

  <body>
    <div class="box">
      <h1>Area of a Rectangle</h1>

      <form method="POST">
        {% csrf_token %} Length :
        <input type="number" name="length" value="{{ length|default:0 }}" /> (in
        m) <br /><br />

        Breadth :
        <input type="number" name="breadth" value="{{ breadth|default:0 }}" />
        (in m) <br /><br />

        <button type="submit">Calculate</button>
        <br /><br />

        Area :
        <input type="text" value="{{ area|default:0 }}" readonly /> m<sup
          >2</sup
        >
      </form>
    </div>
  </body>
</html>
```

## SERVER SIDE PROCESSING:
![alt text](math-1cc.png)

## HOMEPAGE:
![alt text](math.png)

## RESULT:
The program for performing server side processing is completed successfully.
