# Ex.08 Design of Interactive Image Gallery
## Date:

## AIM:
To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for positioning and styling.

### Step 4:
Write JavaScript program for implementing interactivity.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
index.html
```
<html>
<head>
    <title>INTERACTIVE IMAGE GALLERY</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: lightsalmon;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
        }
        .gallery-container {
            max-width: 800px;
            margin: 20px auto;
            overflow: hidden;
            position: relative;
        }
        .gallery-slider {
            display: flex;
            transition: transform 0.5s ease;
        }
        .gallery-item {
            min-width: 100%;
            box-sizing: border-box;
        }
        .gallery-item img {
            width: 100%;
            display: block;
            border-radius: 10px;
        }
        .navigation {
            position: absolute;
            top: 50%;
            width: 100%;
            display: flex;
            justify-content: space-between;
            transform: translateY(-50%);
        }
        .navigation button {
            background-color: rgba(0, 0, 0, 0.5);
            color: white;
            border: none;
            padding: 10px;
            cursor: pointer;
            border-radius: 50%;
            font-size: 18px;
        }
        .navigation button:hover {
            background-color: rgba(0, 0, 0, 0.8);
        }
        h1 {
            text-align: center;
            margin-bottom: 20px;
        }
        footer {
            margin-top: 20px;
            font-size: 16px;
            color: #333;
        }
    </style>
</head>
<body>
    <h1>NANDA IMAGE GALLERY</h1>
    <div class="gallery-container">
        <div class="gallery-slider" id="slider">
            <div class="gallery-item">
                <img src="vijay.jpg" alt="VIJAY">
            </div>
            <div class="gallery-item">
                <img src="sec.jpg" alt="SAVEETHA ENGINEERING COLLEGE">
            </div>
            <div class="gallery-item">
                <img src="zuck.jpg" alt="MARK ZUCKERBURG">
            </div>
            <div class="gallery-item">
                <img src="tata.jpg" alt="RATAN TATA">
            </div>
            <div class="gallery-item">
                <img src="nakamoto.jpg" alt="SATOSHI NAKAMOTO">
            </div>
            <div class="gallery-item">
                <img src="musk.jpg" alt="ELON MUSK">
            </div>
            <div class="gallery-item">
                <img src="kalam.jpg" alt="DR. APJ ABDUL KALAM">
            </div>
        </div>
        <div class="navigation">
            <button id="prev">&#10094;</button>
            <button id="next">&#10095;</button>
        </div>
    </div>

    <footer>
        NANDA KISHOR 24011485
    </footer>

    <script>
        var slider = document.getElementById('slider');
        var prev = document.getElementById('prev');
        var next = document.getElementById('next');

        var currentIndex = 0;
        var totalItems = slider.children.length;

        function updateSlider() {
            slider.style.transform = 'translateX(-' + (currentIndex * 100) + '%)';
        }

        prev.onclick = function() {
            if (currentIndex > 0) {
                currentIndex--;
            } else {
                currentIndex = totalItems - 1;
            }
            updateSlider();
        };

        next.onclick = function() {
            if (currentIndex < totalItems - 1) {
                currentIndex++;
            } else {
                currentIndex = 0;
            }
            updateSlider();
        };
    </script>
</body>
</html>
```

## OUTPUT:

![Screenshot (19)](https://github.com/user-attachments/assets/b1b2c866-9c4a-4553-823c-fd1d25833c7a)


![Screenshot (20)](https://github.com/user-attachments/assets/5c61883a-af36-4077-829e-bde7c2433af3)


![WhatsApp Image 2025-04-12 at 11 30 45_fd17de8d](https://github.com/user-attachments/assets/6126a4d1-d2e7-4bc2-aaa2-661cac4581a0)


![WhatsApp Image 2025-04-12 at 11 30 57_04891593](https://github.com/user-attachments/assets/6170ae63-9e11-43ec-aebe-8447dd0fefaa)


![WhatsApp Image 2025-04-12 at 11 31 09_6940e4a6](https://github.com/user-attachments/assets/0233d14e-bbab-49aa-83ec-66bbe2b5329c)


![Uploading WhatsApp Image 2025-04-12 at 11.31.23_13115506.jpg…]()


## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
