# processing
void setup() {
  size(800, 300);
  textSize(128);
}

int i, dir=1, sp=1;
void draw() {
  fill(255);
  background(0, 0, 0);
  text("Graphics", i, 200);
  if (i>width-535) dir=-1;
  if (i<0) dir=1;
  i = i+dir*sp;
  // if(keyPressed) sp=key-'0';
}
void keyPressed(){
  sp = key - '0';
}
