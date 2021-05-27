## twitter016 | #つぶやきProcessing 
https://twitter.com/nicolasbaez/status/1394477791782047748?s=20

![twitter](https://github.com/nicolasbaez/twitter016/blob/main/twitter016.gif)
```processing
int i, w=500;
float y[]=new float[99];
void setup() {
  size(500, 500);
}
void draw() {
  fill(0, 4);
  rect(0, 0, w, w);
  for (i=0; i<99; i++) {
    stroke(255, noise(y[i])*32);
    point(w*0.585+noise(y[i])*16, y[i]);
    y[i]-=random(4);
    if (y[i]<0)
      y[i]=w*0.8;
  }
  stroke(0);
  line(0, w*0.5, w*0.595, w*0.8);
}
```
