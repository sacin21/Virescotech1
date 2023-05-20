# program to draw a CO2 molecule split
Cheminformatics1
import java.awt.*;
import java.awt.geom.*;

public class CO2Split {

    public static void main(String[] args) {
        // Create a new frame.
        Frame frame = new Frame("CO2 Split");

        // Create a new canvas.
        Canvas canvas = new Canvas();

        // Create a new graphics context.
        Graphics2D g2d = (Graphics2D) canvas.getGraphics();

        // Set the drawing color to black.
        g2d.setColor(Color.black);

        // Draw the CO2 molecule.
        drawCO2Molecule(g2d);

        // Add the canvas to the frame.
        frame.add(canvas);

        // Set the frame's size and make it visible.
        frame.setSize(400, 400);
        frame.setVisible(true);
    }

    private static void drawCO2Molecule(Graphics2D g2d) {
        // Draw the carbon atom.
        g2d.drawOval(100, 100, 50, 50);

        // Draw the oxygen atoms.
        g2d.drawOval(125, 125, 25, 25);
        g2d.drawOval(75, 125, 25, 25);

        // Draw the bonds between the carbon atom and the oxygen atoms.
        g2d.drawLine(100, 150, 125, 125);
        g2d.drawLine(100, 150, 75, 125);
    }
}
