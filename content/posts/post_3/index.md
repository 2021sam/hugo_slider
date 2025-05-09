+++
date = '2025-05-08T23:32:42-07:00'
draft = true
title = 'Post_3'
+++

<style>
/* Style for the image thumbnail */
.thumbnail {
  width: 100%;
  max-width: 300px;
  cursor: pointer;
  transition: 0.3s;
}

.thumbnail:hover {
  opacity: 0.7;
}

/* Modal (hidden by default) */
.modal {
  display: none;
  position: fixed;
  z-index: 1;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  overflow: auto;
  background-color: rgba(0, 0, 0, 0.9);
  padding-top: 60px;
}

/* Modal content */
.modal-content {
  margin: auto;
  display: block;
  width: 80%;
  max-width: 700px;
}

/* Caption (image description) */
#caption {
  text-align: center;
  color: #ccc;
  font-size: 1.2em;
  margin-top: 15px;
}

/* Close button */
.close {
  position: absolute;
  top: 10px;
  right: 25px;
  color: #fff;
  font-size: 35px;
  font-weight: bold;
  transition: 0.3s;
}

.close:hover,
.close:focus {
  color: #bbb;
  text-decoration: none;
  cursor: pointer;
}
</style>

<script>
  // Get the modal
  var modal = document.getElementById("imageModal");

  // Get the image and insert it inside the modal
  var img = document.querySelector(".thumbnail");
  var modalImg = document.getElementById("modalImage");
  var captionText = document.getElementById("caption");

  img.onclick = function() {
    modal.style.display = "block";
    modalImg.src = this.src;
    captionText.innerHTML = this.alt;
  }

  // Get the <span> element that closes the modal
  var span = document.getElementsByClassName("close")[0];

  // When the user clicks on <span> (x), close the modal
  span.onclick = function() {
    modal.style.display = "none";
  }

  // Close the modal if the user clicks outside of the modal
  window.onclick = function(event) {
    if (event.target == modal) {
      modal.style.display = "none";
    }
  }
</script>


## Introduction

This is **bold** text, and this is *emphasized* text.

Visit the [Hugo](https://gohugo.io) website!


![Surf Image](surf1.png)


<!-- Image that will open in a modal when clicked -->
<div class="image-container">
  <img src="./surf1.png" alt="Surf Image" class="thumbnail">
</div>

<!-- Modal Structure -->
<div id="imageModal" class="modal">
  <span class="close">&times;</span>
  <img class="modal-content" id="modalImage">
  <div id="caption"></div>
</div>
