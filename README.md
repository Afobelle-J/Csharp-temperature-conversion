# Csharp-temperature-conversion

this code is written with c sharp to convert from fahrenheit to kelvin, to Celsius, to Rankine and vice versa
using System;

namespace MyApplication
{
  class Program
  {
    static void Main(string[] args)
    {
            string inputUnit, outputUnit;
        double inputValue, outputValue;
        Console.Write("Enter input value: ");
       inputValue = Convert.ToDouble(Console.ReadLine());
         Console.Write("Enter input unit: ");
     inputUnit = Console.ReadLine();
        Console.Write("Enter output unit: ");
        outputUnit = Console.ReadLine();
        Console.Write(inputValue+ inputUnit+"="+ outputUnit);


        if(inputUnit=="F")
        {
        if(outputUnit=="F")
        {outputValue=inputValue;
        Console.Write(inputValue+ inputUnit+"="+ outputValue+ outputUnit);
        }
        else if (outputUnit=="K")
        
    
{outputValue=(inputValue-32)*(8/9)+273.15;
        Console.Write(inputValue+ inputUnit+"="+ outputValue+ outputUnit);
        
        }
        else if (outputUnit=="C")
        
        
        {outputValue=(inputValue-32)*(8/9);
        Console.Write(inputValue+ inputUnit+"="+ outputValue+ outputUnit);
        
        }
        else if (outputUnit=="R")
        
        
        {outputValue=(inputValue+459.67);
        Console.Write(inputValue+ inputUnit+"="+ outputValue+ outputUnit);
        
        }
        }
      

  else if(inputUnit=="K")
        {
        if(outputUnit=="F")
        {outputValue=((inputValue-273.15)*1.8)+32;
Console.Write(inputValue+ inputUnit+"="+ outputValue+ outputUnit);
        }
        else if (outputUnit=="K")
        {outputValue=(inputValue);
        Console.Write(inputValue+ inputUnit+"="+ outputValue+ outputUnit);
        
        }
        else if (outputUnit=="C")
        
        
        {outputValue=(inputValue-273.15);
        Console.Write(inputValue+ inputUnit+"="+ outputValue+ outputUnit);
        }
        else if (outputUnit=="R")
        
        
        {outputValue=(inputValue*1.8);
        Console.Write(inputValue+ inputUnit+"="+ outputValue+ outputUnit);
        }
        }
    

    else if(inputUnit=="C
  {
        if(outputUnit=="F")
        {outputValue=((inputValue*1.8)+32);
        Console.Write(inputValue+ inputUnit+"="+ outputValue+ outputUnit);
        }
        else if (outputUnit=="K")
        {outputValue=(inputValue+273.15);
        Console.Write(inputValue+ inputUnit+"="+ outputValue+ outputUnit);
        }
        else if (outputUnit=="C")
        
        
        {outputValue=(inputValue);
        Console.Write(inputValue+ inputUnit+"="+ outputValue+ outputUnit);
        }
        else if (outputUnit=="R")
        
        
        {outputValue=((inputValue*1.8)+491.67);
        Console.Write(inputValue+ inputUnit+"="+ outputValue+ outputUnit);
        }
       }

     
   else if(inputUnit=="R")
        {
        if(outputUnit=="F")
        {
        outputValue=inputValue+459.67;
        Console.Write(inputValue+ inputUnit+"="+ outputValue+ outputUnit);
        }
        else if (outputUnit=="K")
        {outputValue=(inputValue*(5/9));
        Console.Write(inputValue+ inputUnit+"="+ outputValue+inputUnit+"="+ outputValue+ outputUnit);
        }
        else if (outputUnit=="C")
        
        
        {outputValue=(inputValue-491.67)*(5/9);
        Console.Write(inputValue+ inputUnit+"="+ outputValue+ outputUnit);
        }
        else if (outputUnit=="R")
        
        {outputValue=inputValue;
        Console.Write(inputValue+ inputUnit+"="+ outputValue+ outputUnit);
        }
        }
      
  else
        Console.WriteLine("Out of range");
        }
  }
}
