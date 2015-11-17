# p5.js-Sketch
// for red, green, and blue color values
var r, g, b;

function setup() {
  createCanvas(windowWidth, windowHeight);
  // Pick colors randomly
  r = random(255);
  g = random(255);
  b = random(255);
  frameRate(170);
}

function draw() {
  background('rgba(100%m0%m100%,0.5)');
  colorMode(HSB, 100);
  // Draw a circle
  strokeWeight(2);
  stroke(r, g, b);
  fill(r, g, b, 127);
  translate(width/2, height/2);
  rotate(PI/4.0);
  ellipse(-26, -26, 150, 80);
  rotate(PI/180);
  ellipse(360, 200, 150, 80);
  ellipse(250, 200, 80, 150);
  ellipse(140, 200, 80, 150);
  ellipse(470, 40, 150, 80);
  ellipse(580, 200, 150, 80);
  ellipse(800, 400, 80, 40);
  ellipse(600 ,800, 40, 90);
  ellipse(200, 100, 70, 100);
  ellipse(100, 500, 130, 70);
  ellipse(100, 100, 200, 120);
  ellipse(30, 700, 150, 40);
  ellipse(900, 800, 80, 150);
  ellipse(200, 690, 50, 90);
  ellipse(960, 20, 80, 180);
  ellipse(30, 400, 30, 80);
  ellipse(390, 100, 50, 90);
  
  
  noFill();
  stroke(255, 102, 0);
  //line(85, 20, 10, 0);
  //line(150, 100, 15, 10);
  stroke(10, 0, 100);
  //bezier(300, 70, 250, 270, 150, 560, -10, -300);
  //noLoop();
}

// When the user clicks the mouse
function mousePressed() {
	loop();
  // Check if mouse is inside the circle
var  d = dist(mouseX, mouseY, 500, 500);
  if (d < 100) {
    // Pick new random color values
    r = random(255);
    g = random(255);
    b = random(255);
    //loop();
  }
}
