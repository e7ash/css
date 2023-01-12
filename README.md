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
body {
  font-family: sans-serif;
  color: red;
}

h1 {
  color: black;
  font-size: 2em;
  font-family: Georgia, 'Times New Roman', Times, serif;
  border: 8px solid red;
  display: inline;

}

h2 {
  font-size: 1.5em;
  color: black;
}

.job-title {
  color: black;
  font-weight: bold;
}

a:link,
a:visited {
  color: red;
}

a:hover {
  text-decoration: none;
}
<script>
