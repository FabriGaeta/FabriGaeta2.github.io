.emscripten {
  padding: 0;
  padding-right: 0;
  margin-left: auto;
  margin-right: auto;
  display: block;
  overflow: hidden;
  border-radius: 6px;
}

textarea.emscripten {
  resize: none;
  margin: 6px auto;
  border: 0px none;
  padding: 6px;
  font-family: monospace;
  font-stretch: condensed;
  font-size: small;
  width: 588px;
  /* 600px - borders */
  border-radius: 6px;
  background: #e7e8ea
}

div.emscripten {
  text-align: center;
}

/* div.emscripten_border { border: 1px solid black; } */
/* the canvas *must not* have any border or padding, or mouse coords will be wrong */
canvas.emscripten {
  display: none;
  border: 0px none;
  background-color: #00000000;
  width: 600px;
  height: 600px;

  image-rendering: optimizeSpeed;
  image-rendering: -moz-crisp-edges;
  image-rendering: -o-crisp-edges;
  image-rendering: -webkit-optimize-contrast;
  image-rendering: optimize-contrast;
  image-rendering: crisp-edges;
  image-rendering: pixelated;
  -ms-interpolation-mode: nearest-neighbor;
}

progress {
  margin: 0px auto;
  border: 0px none;
  border-radius: 25px;
  height: 6px;
  width: 120px;
  background-color: rgb(220, 220, 220);
  color: #aaa;
}

progress::-webkit-progress-bar {
  border-radius: 35px;
  background-color: rgb(220, 220, 220);
  width: 100%;
}

progress::-webkit-progress-value {
  border-radius: 35px;
  background-color: #aaa !important;
}

progress::-moz-progress-bar {
  border-radius: 25px;
  background-color: #aaa !important;
}

.spinner {
  height: 20px;
  width: 20px;
  margin: 0px auto;
  -webkit-animation: rotation .6s linear infinite;
  -moz-animation: rotation .6s linear infinite;
  -o-animation: rotation .6s linear infinite;
  animation: rotation 0.6s linear infinite;
  border-left: 6px solid rgb(220, 220, 220);
  border-right: 6px solid rgb(220, 220, 220);
  border-bottom: 6px solid rgb(220, 220, 220);
  border-top: 6px solid #aaa;
  border-radius: 100%;
  background-color: rgba(255, 255, 255, 0);
}

@-webkit-keyframes rotation {
  from {
    -webkit-transform: rotate(0deg);
  }

  to {
    -webkit-transform: rotate(360deg);
  }
}

@-moz-keyframes rotation {
  from {
    -moz-transform: rotate(0deg);
  }

  to {
    -moz-transform: rotate(360deg);
  }
}

@-o-keyframes rotation {
  from {
    -o-transform: rotate(0deg);
  }

  to {
    -o-transform: rotate(360deg);
  }
}

@keyframes rotation {
  from {
    transform: rotate(0deg);
  }

  to {
    transform: rotate(360deg);
  }
}
