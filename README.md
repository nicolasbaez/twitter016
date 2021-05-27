# twitter016
#つぶやきProcessing int i,w=500;float y[]=new float [99];void setup(){size(500,500);}void draw(){fill(0,4);rect(0,0,w,w);for(i=0;i&lt;99;i++){stroke(255,noise(y[i])*32);point (w*0.585+noise(y[i])*16,y[i]);y[i]-=random(4);if(y[i]&lt;0)y[i]=w*0.8;}stroke(0);line(0,w*0.5,w*0.595,w*0.8);}
