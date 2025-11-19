# Ex.08 Design of Interactive Image Gallery

## AIM
  To design a web application for an inteactive image gallery with minimum five images.

## DESIGN STEPS

## Step 1:

Clone the github repository and create Django admin interface

## Step 2:

Change settings.py file to allow request from all hosts.

## Step 3:

Use CSS for positioning and styling.

## Step 4:

Write JavaScript program for implementing interactivit

## Step 5:

Validate the HTML and CSS code

## Step 6:

Publish the website in the given URL.

## PROGRAM
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Interactive Image Gallery</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 20px;
      background-color: #f4f4f4;
      text-align: center;
    }
    h1 {
      text-align: center;
    }
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 10px;
      margin-top: 20px;
      justify-items: center;
    }
    .gallery img {
      width: 80%;
      border-radius: 8px;
      cursor: pointer;
      transition: transform 0.3s;
    }
    .gallery img:hover {
      transform: scale(1.05);
    }
  </style>
</head>
<body>
  <h1>Interactive Image Gallery</h1>
  <div class="gallery">
    <img src="c:\Users\lenovo\Downloads\download (10).jpg" alt="Image 1" onclick="openImage(this.src)">
    <img src="c:\Users\lenovo\Downloads\download (6).jpg" alt="Image 2" onclick="openImage(this.src)">
    <img src="c:\Users\lenovo\Downloads\Chasing freedom_.jpg" alt="Image 3" onclick="openImage(this.src)">
    <img src="c:\Users\lenovo\Downloads\download (7).jpg" alt="Image 4" onclick="openImage(this.src)">
    <img src="c:\Users\lenovo\Downloads\🔮.jpg" alt="Image 5" onclick="openImage(this.src)">
    <img src="c:\Users\lenovo\Downloads\download (8).jpg" alt="Image 6" onclick="openImage(this.src)">
    <img src="c:\Users\lenovo\Downloads\Aesthetic Photos.jpg" alt="Image 7" onclick="openImage(this.src)">
    <img src="c:\Users\lenovo\Downloads\download (9).jpg" alt="Image 7" onclick="openImage(this.src)">
  </div>

  <script>
    function openImage(imgSrc) {
      const newWindow = window.open('', '_blank');
      newWindow.document.write(`
        <html>
        <head>
          <title>View Image</title>
          <style>
            body {
              background-color: #f4f4f4;
              display: flex;
              justify-content: center;
              align-items: center;
              height: 100vh;
              margin: 0;
            }
            img {
              max-width: 80%;
              max-height: 80vh;
              border-radius: 10px;
              box-shadow: 0 4px 10px rgba(0,0,0,0.3);
            }
          </style>
        </head>
        <body>
          <img src="${imgSrc}" alt="Opened Image">
        </body>
        </html>
      `);
    }
  </script>
</body>
</html>
```

## OUTPUT
![alt text](<Screenshot 2025-11-19 100651.png>)
## RESULT
  The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
