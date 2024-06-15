using System;

public class EchoingCanyon
{
    // Fields, properties, and methods can be defined here
    private string canyonName;
    private int echoStrength;

    // Constructor
    public EchoingCanyon(string name, int strength)
    {
        canyonName = name;
        echoStrength = strength;
    }

    // Method to echo a message
    public void EchoMessage(string message)
    {
        for (int i = 0; i < echoStrength; i++)
        {
            Console.WriteLine(message);
        }
    }

    // Example of a property
    public string CanyonName
    {
        get { return canyonName; }
        set { canyonName = value; }
    }

    // Example of a method
    public void DescribeCanyon()
    {
        Console.WriteLine($"This is {canyonName}, known for its echoing effect with strength {echoStrength}.");
    }

    // Main method for testing
    public static void Main(string[] args)
    {
        // Create an instance of EchoingCanyon
        EchoingCanyon canyon = new EchoingCanyon("Echoing Canyon", 3);

        // Demonstrate its usage
        canyon.DescribeCanyon();
        canyon.EchoMessage("Hello, world!");
    }
}
