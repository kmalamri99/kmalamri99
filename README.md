- 👋 Hi, I’m @kmalamri99
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
kmalamri99/kmalamri99 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
// This code will draw a line
#include<GL/glut.h>
void init()
{​​​​
glClearColor(1,1,1,1);
gluOrtho2D(0,400,0,400);
}​​​​
void draw()
{​​​​
glClear(GL_COLOR_BUFFER_BIT);
glColor3f(1,0,0);
glBegin(GL_LINES);
 glVertex2f(50,50);
glVertex2f(150,100);
glColor3f(1,1,0);
glBegin(GL_LINES);
 
 glVertex2f(50,80);
glVertex2f(300,300);
glColor3f(0,1,0);
glBegin(GL_LINES);
 
 glVertex2f(50,50);
glVertex2f(300,300);
glEnd();
glFlush();
}​​​​
int main(int argc, char *argv[])
{​​​​
        glutInit(&argc, argv);
 
glutInitDisplayMode(GLUT_SINGLE|GLUT_RGB);
glutInitWindowPosition(0,0);
glutInitWindowSize(400,400);
glutCreateWindow("Exercise1 to draw a line");
init();
glutDisplayFunc(draw);
glutMainLoop();
return 0;
}
