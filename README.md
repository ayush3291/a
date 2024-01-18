<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>css card hover effects | untoldcoding</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <div class="container">
      <div class="untoldcoding">
        <div class="img-container">
          <img
            src="https://i.postimg.cc/ZKhfkqhD/Black-And-Gold-Happy-Birthday-Document-A4.png"
            alt=""
          />
        </div>
        <div class="untoldcoding-details">
          <h2>Birthday Wishes</h2>
          Happy Birthday to you.
          You’re more than just a friend to me.
          May your birthday be as fantastic and special as you are,
          filled with joy, love, and endless happy moments.❤️❤️❤️

          <br /><br />
          ---Ayush
        </div>
      </div>
    </div>
  </body>
</html>
body {
  margin: 0;
  padding: 0;
  background: #f2f2f2;
  font-family: "Acme";
  background: #000;
}

.container {
  max-width: 1000px;
  margin: 100px auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
}

.untoldcoding {
  position: relative;
  margin: 20px 0;
  width: 300px;
  height: 400px;
  background: linear-gradient(#fef7f7, #9198e5);
  transform-style: preserve-3d;
  transform: perspective(2000px);
  transition: 1s;
}

.untoldcoding:hover {
  z-index: 1111;
  transform: perspective(2000px) rotate(-10deg);

  box-shadow: 5px 5px 20px rgb(235, 151, 128);
}

.untoldcoding .img-container {
  position: relative;
  width: 100%;
  height: 100%;
  border: 1px solid #000;
  box-sizing: border-box;
  transform-origin: left;
  z-index: 1;
  transition: 1s;
}

.untoldcoding .img-container img {
  position: absolute;
  left: 0;
  top: 0;
  height: 100%;
  width: 100%;
  object-fit: cover;
}

.untoldcoding:hover .img-container {
  transform: rotateY(-135deg);
}

.untoldcoding .untoldcoding-details {
  position: absolute;
  left: 0;
  top: 0;
  box-sizing: border-box;
  padding: 20px;
  color: #000;
}

.untoldcoding .untoldcoding-details h2 {
  margin: 0;
  padding: 0.5em 0;
  text-transform: uppercase;
  font-size: 2em;
  background: linear-gradient(to right, #f32170, #ff0c08, #710071, #eedd44);
  -webkit-text-fill-color: transparent;
  -webkit-background-clip: text;
  animation: untold 3s infinite ease-in-out;
}

@keyframes untold {
  0% {
    background: linear-gradient(to right, #f32170, #ff0c08, #710071, #eedd44);
    -webkit-text-fill-color: transparent;
    -webkit-background-clip: text;
    animation: untold 0.1s infinite ease-in-out;
  }
  50% {
    background: linear-gradient(to right, #2fff00, #1008ff, #ec4705, #a744ee);
    -webkit-text-fill-color: transparent;
    -webkit-background-clip: text;
    animation: untold 3s infinite ease-in-out;
  }
  100% {
    background: linear-gradient(to right, #f32121, #ff0890, #cdb903, #d122f8);
    -webkit-text-fill-color: transparent;
    -webkit-background-clip: text;
    animation: untold 1s infinite ease-in-out;
  }
}
.untoldcoding .untoldcoding-details p {
  margin: 0;
  padding: 0;
  line-height: 25px;
  font-size: 1.3em;
  font-weight: 900;
}
