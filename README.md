# Ex.08 Design of Interactive Image Gallery
## Date: 18/12/2025

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
```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Interactive Image Gallery</title>
<style>
body { font-family: Arial; text-align: center; background: #f0f0f0; }
.gallery { display: flex; flex-wrap: wrap; justify-content: center; gap: 10px; margin-top: 20px; }
.gallery img { width: 200px; height: 150px; object-fit: cover; cursor: pointer; border-radius: 8px; transition: transform 0.2s; }
.gallery img:hover { transform: scale(1.1); }

/* Modal Styles */
.modal { display: none; position: fixed; z-index: 1; padding-top: 50px; left: 0; top: 0; width: 100%; height: 100%; overflow: auto; background-color: rgba(0,0,0,0.9); }
.modal-content { margin: auto; display: block; max-width: 80%; }
.close { position: absolute; top: 20px; right: 35px; color: #fff; font-size: 40px; font-weight: bold; cursor: pointer; }
</style>
</head>
<body>

<h1>THE FAB FOUR GALLERY</h1>
<div class="gallery">
    
    <img src="root.jpg" alt="Image 1" onclick="openModal(this)">
    <img src="kohli.jpg" alt="Image 2" onclick="openModal(this)">
    <img src="smith.jpg" alt="Image 3" onclick="openModal(this)">
    <img src="kane.avif" alt="Image 4" onclick="openModal(this)">
   

    
</div>

<!-- Modal -->
<div id="myModal" class="modal">
  <span class="close" onclick="closeModal()">&times;</span>
  <img class="modal-content" id="modalImg">
</div>

<script>
function openModal(img) {
    document.getElementById("myModal").style.display = "block";
    document.getElementById("modalImg").src = img.src;
}
function closeModal() {
    document.getElementById("myModal").style.display = "none";
}
</script>

</body>
</html>
```
## OUTPUT:
![alt text](<Screenshot (92).png>)

![alt text](<Screenshot (93).png>)
## RESULT:
The program for designing an interactive image gallery using HTML, CSS and JavaScript is executed successfully.
