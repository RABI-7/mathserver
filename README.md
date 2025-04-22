# Ex.05 Design a Website for Server Side Processing
# Date:12/04/2025
# AIM:
To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side.

# FORMULA:
P = I2R
P --> Power (in watts)
 I --> Intensity
 R --> Resistance

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Create python programs for views and urls to perform server side processing.

## Step 5:
Create a HTML file to implement form based input and output.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lamp Filament Power Calculator</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: url("Screenshot 2024-10-28 115234.png");
            margin: 0;
            padding: 0;
        }

        .container {
            max-width: 600px;
            margin: 90px auto;
            padding: 20px;
            background-color: cyan;
            box-shadow: 0 0 10px rgb(0, 0, 0);
            border-radius: 10px;
        }

        h1 {
            text-align: center;
            color: black;
        }

        .input-group {
            margin-bottom: 30px;
        }

        label {
            display: block;
            font-weight: bold;
            color: rgb(117, 125, 239);
            margin-bottom: 5px;
        }

        input[type="number"] {
            width: 90%;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }

        button {
            width: 100%;
            padding: 10px;
            background-color: #f4f0d2;
            color: #fff;
            border: none;
            border-radius: 4px;
            font-size: 16px;
            cursor: pointer;
        }

        button:hover {
            background-color: #0056b3;
        }

        .result {
            margin-top: 20px;
            font-size: 18px;
            text-align: center;
            color: #333;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Lamp Filament Power Calculator</h1>
        <div class="input-group">
            <label for="current">Current (I) in Amps:</label>
            <input type="number" id="current" placeholder="Enter current (in Amps)" required>
        </div>
        <div class="input-group">
            <label for="resistance">Resistance (R) in Ohms:</label>
            <input type="number" id="resistance" placeholder="Enter resistance (in Ohms)" required>
        </div>
        <button onclick="calculatePower()">Calculate Power</button>
        <div class="result" id="result"></div>
    </div>

    <script>
        function calculatePower() {
            var current = document.getElementById('current').value;
            var resistance = document.getElementById('resistance').value;
            if (current && resistance) {
                var power = Math.pow(current, 2) * resistance;
                document.getElementById('result').innerHTML = 'Power (P) = ' + power.toFixed(2) + ' Watts';
            } else {
                document.getElementById('result').innerHTML = 'Please enter valid values for current and resistance.';
            }
        }
    </script>
</body>
</html>

```
# SERVER SIDE PROCESSING:
![ChatGPT Image Apr 12, 2025, 12_13_30 AM](https://github.com/user-attachments/assets/f74bcb07-8662-4d6d-87ca-92318a35f432)




# HOMEPAGE:
![Screenshot (80)](https://github.com/user-attachments/assets/f4a87abf-e297-494e-bb2e-ba0775147f8e)
![Screenshot (86)](https://github.com/user-attachments/assets/15e9e850-62ee-4f5c-8dc3-a0ee918dd439)



# RESULT:
The program for performing server side processing is completed successfully.
