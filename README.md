# Java program to show the reaction of CO2 molecule with NaOH
Cheminformatics1
import java.util.Scanner;

public class CO2NaOHReaction {

  public static void main(String[] args) {
    Scanner scanner = new Scanner(System.in);

    // Get the concentration of CO2 in the air.
    System.out.println("Enter the concentration of CO2 in the air (in mol/L): ");
    double co2Concentration = scanner.nextDouble();

    // Get the concentration of NaOH in the solution.
    System.out.println("Enter the concentration of NaOH in the solution (in mol/L): ");
    double naohConcentration = scanner.nextDouble();

    // Calculate the equilibrium constant.
    double equilibriumConstant = 1e-6;

    // Calculate the equilibrium concentrations.
    double na2co3Concentration = equilibriumConstant * co2Concentration * naohConcentration;
    double h2oConcentration = equilibriumConstant * co2Concentration * naohConcentration;

    // Print the results.
    System.out.println("The concentration of Na2CO3 in the solution is " + na2co3Concentration + " mol/L.");
    System.out.println("The concentration of H2O in the solution is " + h2oConcentration + " mol/L.");
  }
}
