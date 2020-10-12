# Métodos

## Métodos státicos

 Un método estático juega un papel similar a una función común en otros lenguajes
 
 Los métodos estáticos dentro de la misma clase se pueden llamar como funciones en otros lenguajes, por lo que no se requieren puntos.
 
 > Es como crear funciones normales en otro lenguaje por q lo declaramos fuera del main y podemos llamarlos con sus nombres nada más.
 
 ```java
 import com.educative.graphics.*;

class SmileyFactored {
  static Canvas c;
  
  public static void drawOutline() {
    // Draw the outline of the face
    c.fill("yellow");
    c.stroke("black");
    c.circle(100, 100, 50);
  }
  
  public static void drawMouth() {
    // draw the mouth
    c.stroke("black");
    c.fill("yellow");
    c.circle(100, 100, 30);
    c.stroke("yellow");
    c.rect(68, 68, 62, 40);
  }
  
  public static void drawEyes() {
    // draw the eyes
    c.stroke("black");
    c.fill("black");
    c.circle(100 - 20, 100 - 10, 5);
    c.circle(100 + 20, 100 - 10, 5);
  }
  
  public static void main(String[] args) {
   
    c = new Canvas(200, 200);
    
    drawOutline();
    drawMouth();
    drawEyes();
    
    c.draw();
  }
}
```
