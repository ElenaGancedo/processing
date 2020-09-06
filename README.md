# processing
// creative codec
// Design multitriangles
//triangle(x1, y1, x2, y2, x3, y3);

void setup() {
  size(840, 640);
   background(random(255));
 //background(random(255), random(255),random(255),100); 
 colorMode(HSB, width, height, 50);
 // noFill();
 frameRate(5);
}
void draw() { 
   for(int i=0; i<100; i++) {
    drawX(int(random(8)), int(random(width)), int(random(height)), int(random(80)), int(random(40)));
  }
}
  void drawX(int grosor, int x, int y, int size1,int size2 ) {
  strokeWeight(random(grosor));
 // stroke(mouseX, width, width);
  stroke(random(355), random(355),random(355));
  fill(mouseX, width, width,80);
 // triangle(x+size1,y,x,y+size1,x+size2,y);
 // triangle(x+size1,y+size2,x,y+size1,x+size2,y);
   triangle(x,y+size2,x+size2,y+size2,x+size2,y);
  stroke(mouseY, height, height);
  fill(mouseX, height, height,80);
  //fill(random(355), random(355),random(355),100);
  triangle(x+size2,y,x,y,x+size2,y+size2);

}
void mousePressed(){
  saveFrame("triang####.png");                                            
}  
