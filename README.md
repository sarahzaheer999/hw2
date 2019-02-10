# hw2


# Piet Mondrian-Version 1

function setup() {
    createCanvas(400, 400);
}

function draw() {
    background(240);
    noStroke();
    strokeCap(SQUARE);

    // blue square
    fill(0, 0, 255);
    rect(200, 250, 120, 400);

    // red square
    fill(255, 0, 0);
    rect(0, 0, 200, 100);

    // yellow square
    fill(255, 255, 0);
    rect(0, 250, 40, 400);

   stroke(0);
   strokeWeight(10);
   line(200, 0, 200, 400); 
	 line(0, 100, 400, 100);
	 line(0, 250, 400, 250);
   line(40, 400, 40, 250);
	 line(320, 250, 320, 400); 

   
    
}

# Piet Mondrian-Version 2

function setup() {
    createCanvas(400, 400);
}

function draw() {
    background(240);
    noStroke();
    strokeCap(SQUARE);

    // blue square
    fill(0, 0, 255);
    rect(300, 120, 200, 120);

    // red square
    fill(255, 0, 0);
    rect(0, 0, 300, 120);

   

   stroke(0);
   strokeWeight(10);
   line(300, 0, 300, 400); 
	 line(0, 120,400, 120);
	 line(300, 240, 400, 240);
   
	 line(0, 396, 300, 396); 

   
    
}

# Make ball bounce up and down

var circley = 0;
var speed = 5;

function setup() {
  createCanvas(400, 400);
}


function draw() {
  background(220);
  
  fill(255, 255, 0);
  ellipse(180, circley, 100, 100); // Draw yellow ellipse 
  
  
  
  if(circley>height)
    speed=-5
    
  circley=circley+speed
  
   if(circley<= 0)
    speed=5
    
  circley=circley+speed
  
  
}


# Changing the speed of the ball bounce when it touches the top

var circley = 0;
var speed = 1;

function setup() {
  createCanvas(400, 400);
}


function draw() {
  background(220);
  
  fill(255, 255, 0);
  ellipse(180, circley, 100, 100); // Draw yellow ellipse 
  
  
  
  if(circley>height)
    speed=-5
    
  circley=circley+speed
  
   if(circley<= 0)
    speed=50
    
  circley=circley+speed
  
  
}

# Make HSB turn into RGB

function setup() {
    createCanvas(400, 400);
    background(220);
    // RGB 
   colorMode(RGB,250);
}

function draw() {
    let x = random(width);
    let y = random(height);
    fill(x, y, 100);
    noStroke()
    ellipse(x, y, 20);
}

# Changing Variables

var x=h
var y=s

function setup() {
    createCanvas(400, 400);
    background(220);
    // HSB with H range 0-400, S range 0-400, B range 0-100:
    colorMode(HSB, 400, 400, 100);
}

function draw() {
    let h = random(width);
    let s = random(height);
    fill(h, s, 100);
    noStroke()
    ellipse(h, s, 20);
}


Change in variable h,s to dog cat
var x=dog
var y=cat

function setup() {
    createCanvas(400, 400);
    background(220);
    // HSB with H range 0-400, S range 0-400, B range 0-100:
    colorMode(HSB, 400, 400, 100);
}

function draw() {
    let dog = random(width);
    let cat = random(height);
    fill(dog, cat, 100);
    noStroke()
    ellipse(dog, cat, 20);
}


Note:No change,still the same in both;Shows "error"
