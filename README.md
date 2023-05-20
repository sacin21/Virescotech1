# Virescotech1
Cheminformatics1
import java.awt.*;
import java.awt.geom.*;

public class CO2 {

    public static void main(String[] args) {
                                              // Create a new frame
                                              Frame frame = new Frame("CO2 Molecule");

                                              // Create a new canvas
                                              Canvas canvas = new Canvas();

                                              // Set the canvas size
                                                 canvas.setSize(400, 400);

                                              // Add the canvas to the frame
                                                 frame.add(canvas);

                                              // Create a new graphics object
                                              Graphics g = canvas.getGraphics();

                                              // Draw the CO2 molecule
                                                 drawCO2(g);

                                              // Display the frame
                                                frame.setVisible(true);
                                           }

    private static void drawCO2(Graphics g) {
                                              // Set the line width
                                                 g.setLineWidth(2);

                                                  // Set the line color
                                                   g.setColor(Color.black);

                                                 // Draw the carbon atom
                                                   g.drawOval(100, 100, 50, 50);

                                                // Draw the oxygen atoms
                                                 g.drawOval(75, 75, 25, 25);
                                                 g.drawOval(125, 75, 25, 25);

                                               // Draw the bonds between the atoms
                                                 g.drawLine(100, 100, 75, 75);
                                                  g.drawLine(100, 100, 125, 75);
                                           }
}
