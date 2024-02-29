Creating a Graphics Object:
Before you can draw lines, shapes, or images, you need to create a Graphics object. This object represents the drawing surface where you’ll perform your graphical operations.
There are several ways to create a Graphics object:
From the Paint Event:
In the Paint event handler of a form or control, you receive a reference to a Graphics object via the PaintEventArgs.
Example (VB.NET):
Private Sub Form1_Paint(sender As Object, pe As PaintEventArgs) Handles MyBase.Paint
    Dim g As Graphics = pe.Graphics
    ' Insert code to paint the form or control here.
End Sub

Example (C#):
C#

private void Form1_Paint(object sender, PaintEventArgs pe)
{
    Graphics g = pe.Graphics;
    // Insert code to paint the form here.
}
AI-generated code. Review and use carefully. More info on FAQ.
Using CreateGraphics Method:
Call the CreateGraphics method of a control or form to obtain a reference to a Graphics object representing the drawing surface.
Example (C#):
C#

Graphics g;
// Sets 'g' to a Graphics object representing the drawing surface of the control or form.
g = this.CreateGraphics();
AI-generated code. Review and use carefully. More info on FAQ.
From an Existing Image:
You can create a Graphics object from any object that inherits from Image. This is useful when altering an existing image.
Drawing on the Graphics Surface:
Once you have a Graphics object, you can use it to:
Draw lines and shapes.
Render text.
Display and manipulate images.
Remember that the Paint event is a common place to start your graphical operations. Explore different drawing methods and unleash your creativity!
