<html>
  <head>
    <link rel="stylesheet" href="./app.css"/>
    <head>
      <body>
        <div id="app">

<h1>Eli Nicholas Ash</h1>
<p>
  <ul>
    <il>
      <h2>
        Early Life
      </h2>
    </il>
    <p>
      Born May 1, 2002
    </p>
    <p>
      Raised in Parkersburg, Wv
    </p>
    <p>
      Two Brothers Ian & Jon
    </p>
    <p>
      Graduated 2020, Parkersburg High
    </p>
  </ul>
</p>

<p> </p>

<h2>Socials</h2>
<ul>
  <li>Email: <a href="eliwav@aol.com">eliwav@aol.com</a></li>
  <li>Web: <a href="https://theuselessweb.com/">https://theuselessweb.com/</a></li>
  <li>Cell 304-679-8118</li>
</ul>

<label>Image File:</label><br />
<input type="file" id="imageLoader" name="imageLoader" />
<canvas id="imageCanvas"></canvas>

<div *ngFor="let user of users">
    <span> {{ user.name }} </span> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<button ion-button type="button" (click)="openDocument(user.image)"> View Image </button>
    <br>
</div>






<script>
var imageLoader = document.getElementById('imageLoader');
    imageLoader.addEventListener('change', handleImage, false);
var canvas = document.getElementById('imageCanvas');
var ctx = canvas.getContext('2d');


function handleImage(e){
    var reader = new FileReader();
    reader.onload = function(event){
        var img = new Image();
        img.onload = function(){
            canvas.width = img.width: 250;
            canvas.height = img.height: 250;
            ctx.drawImage(img,0,0);
        }
        img.src = event.target.result;
    }
    reader.readAsDataURL(e.target.files[0]);     
}

 users = [
    {
      "name": "First User",
      "image": [
        "https://ionicframework.com/img/ionic-logo-blog.png", "https://ionicframework.com/img/ionic_logo.svg", "https://ionicframework.com/img/ionic-logo-blog.png"
      ]
    },
    {
      "name": "Second User",
      "image": [
        "https://ionicframework.com/img/ionic-logo-blog.png", "https://ionicframework.com/img/ionic_logo.svg", "https://ionicframework.com/img/ionic-logo-blog.png"
      ]
    },
    {
      "name": "Third User",
      "image": [
        "https://ionicframework.com/img/ionic-logo-blog.png", "https://ionicframework.com/img/ionic_logo.svg", "https://ionicframework.com/img/ionic-logo-blog.png"
      ]
    },
  ]

</script>
       
        </html>









