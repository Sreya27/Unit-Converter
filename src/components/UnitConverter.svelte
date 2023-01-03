<script>
    let type = "length";
    let fromValue = 0;
    let fromUnit = "";
    let toUnit = "";
    let result = 0;
    
    function convert() {
      if (type === "length") {
              
        // perform length conversion
              
               if (fromUnit === "meter" && toUnit === "kilometer") {
        result = fromValue * 0.001;
      } else if (fromUnit === "meter" && toUnit === "Centimeter") {
        result = fromValue * 100;
      } else if(fromUnit === "meter" && toUnit === "Nautical-miles"){
        result = fromValue / 1852;
      }
      else if(fromUnit === "meter" && toUnit === "Nanometer"){
        result = fromValue * 1000000000;
      }
      else if(fromUnit === "meter" && toUnit === "Inches"){
        result = fromValue ** 39.37;
      }
      else if(fromUnit === "meter" && toUnit === "Yard"){
        result = fromValue * 1.0936;
      }
      else if(fromUnit === "meter" && toUnit === "Miles"){
        result = fromValue / 1609.34;
      }
      else if(fromUnit === "meter" && toUnit === "Millimeter"){
        result = fromValue * 1000;
      }
      else if(fromUnit === "meter" && toUnit === "Feet"){
        result = fromValue *  3.280;
      }
      else if(fromUnit === "meter" && toUnit === "Micrometer"){
        result = fromValue * 1000000;
      }
              // kilometer 
       if (fromUnit === "kilometer" && toUnit === "meter") {
        result = fromValue * 1000;
      } else if (fromUnit === "kilometer" && toUnit === "Centimeter") {
        result = fromValue * 100000;
      } else if(fromUnit === "kilometer" && toUnit === "kilometer"){
        result = fromValue;
      }
      else if(fromUnit === "kilometer" && toUnit === "Nautical-miles"){
        result = fromValue / 1.852;
      }
      else if(fromUnit === "kilometer" && toUnit === "Nanometer"){
        result = fromValue * 1000000000000;
      }
      else if(fromUnit === "kilometer" && toUnit === "Inches"){
        result = fromValue * 39370.08;
      }
      else if(fromUnit === "kilometer" && toUnit === "Yard"){
        result = fromValue * 1093.61;
      }
      else if(fromUnit === "kilometer" && toUnit === "Miles"){
        result = fromValue / 1.60934;
      }
      else if(fromUnit === "kilometer" && toUnit === "Millimeter"){
        result = fromValue * 1000000;
      }
      else if(fromUnit === "kilometer" && toUnit === "Feet"){
        result = fromValue * 3280.8;
      }
      else if(fromUnit === "kilometer" && toUnit === "Micrometer"){
        result = fromValue * 1000000000;
      }
      
  //convert Centimeter into following units 
      if (fromUnit === "Centimeter" && toUnit === "kilometer") {
        result = fromValue / 100000;
      } else if (fromUnit === "Centimeter" && toUnit === "meter") {
        result = fromValue / 100;
      } else if(fromUnit === "Centimeter" && toUnit === "Centimeter"){
        result = fromValue;
      }
      else if(fromUnit === "Centimeter" && toUnit === "Nautical-miles"){
        result = fromValue / 185200;
      }
      else if(fromUnit === "Centimeter" && toUnit === "Nanometer"){
        result = fromValue * 10000000;
      }
      else if(fromUnit === "Centimeter" && toUnit === "Inches"){
        result = fromValue / 2.54;
      }
      else if(fromUnit === "Centimeter" && toUnit === "Yard"){
        result = fromValue / 91.44;
      }
      else if(fromUnit === "Centimeter" && toUnit === "Miles"){
        result = fromValue / 160934.4;
      }
      else if(fromUnit === "Centimeter" && toUnit === "Millimeter"){
        result = fromValue * 10;
      }
      else if(fromUnit === "Centimeter" && toUnit === "Feet"){
        result = fromValue / 30.48;
      }
      else if(fromUnit === "Centimeter" && toUnit === "Micrometer"){
        result = fromValue * 10000;
      }
     
     
      //convert Nautical-miles into following units 
     if (fromUnit === "Nautical-miles" && toUnit === "kilometer") {
        result = fromValue * 1.852;
      } else if (fromUnit === "Nautical-miles" && toUnit === "meter") {
        result = fromValue * 1852;
      } else if(fromUnit === "Nautical-miles" && toUnit === "Centimeter"){
        result = fromValue;
      }
      else if(fromUnit === "Nautical-miles" && toUnit === "Nautical-miles"){
        result = fromValue ;
      }
      else if(fromUnit === "Nautical-miles" && toUnit === "Nanometer"){
        result = fromValue * 1852000000000;
      }
      else if(fromUnit === "Nautical-miles" && toUnit === "Inches"){
        result = fromValue * 72913.39;
      }
      else if(fromUnit === "Nautical-miles" && toUnit === "Yard"){
        result = fromValue * 2025.371;
      }
      else if(fromUnit === "Nautical-miles" && toUnit === "Miles"){
        result = fromValue * 1.15077944;
      }
      else if(fromUnit === "Nautical-miles" && toUnit === "Millimeter"){
        result = fromValue * 1852000;
      }
      else if(fromUnit === "Nautical-miles" && toUnit === "Feet"){
        result = fromValue * 6076.115;
      }
      else if(fromUnit === "Nautical-miles" && toUnit === "Micrometer"){
        result = fromValue * 1852000000;
      }
  
     //convert Nanometer into following units 
     if (fromUnit === "Nanometer" && toUnit === "kilometer") {
        result = fromValue / 1000000000000;
      } else if (fromUnit === "Nanometer" && toUnit === "meter") {
        result = fromValue / 1000000000;
      } else if(fromUnit === "Nanometer" && toUnit === "Centimeter"){
        result = fromValue / 10000000;
      }
      else if(fromUnit === "Nanometer" && toUnit === "Nautical-miles"){
        result = fromValue / 1852000000000;
      }
      else if(fromUnit === "Nanometer" && toUnit === "Nanometer"){
        result = fromValue ;
      }
      else if(fromUnit === "Nanometer" && toUnit === "Inches"){
        result = fromValue / 25400000;
      }
      else if(fromUnit === "Nanometer" && toUnit === "Yard"){
        result = fromValue / 914400000;
      }
      else if(fromUnit === "Nanometer" && toUnit === "Miles"){
        result = fromValue / 1609344000000;
      }
      else if(fromUnit === "Nanometer" && toUnit === "Millimeter"){
        result = fromValue / 1000000;
      }
      else if(fromUnit === "Nanometer" && toUnit === "Feet"){
        result = fromValue / 304800000;
  
      }
      else if(fromUnit === "Nanometer" && toUnit === "Micrometer"){
        result = fromValue * 1000;
      }
  
  
      //convert Inches into following units 
         if (fromUnit === "Inches" && toUnit === "kilometer") {
        result = fromValue / 39370.0787;
      } else if (fromUnit === "Inches" && toUnit === "meter") {
        result = fromValue / 39.3700787;
      } else if(fromUnit === "Inches" && toUnit === "Centimeter"){
        result = fromValue * 2.54;
      }
      else if(fromUnit === "Inches" && toUnit === "Nautical-miles"){
        result = fromValue / 72913.3858;
      }
      else if(fromUnit === "Inches" && toUnit === "Nanometer"){
        result = fromValue * 25400000;
      }
      else if(fromUnit === "Inches" && toUnit === "Inches"){
        result = fromValue ;
      }
      else if(fromUnit === "Inches" && toUnit === "Yard"){
        result = fromValue / 36;
      }
      else if(fromUnit === "Inches" && toUnit === "Miles"){
        result = fromValue / 63360;
      }
      else if(fromUnit === "Inches" && toUnit === "Millimeter"){
        result = fromValue * 25.4;
      }
      else if(fromUnit === "Inches" && toUnit === "Feet"){
        result = fromValue / 12;
      }
      else if(fromUnit === "Inches" && toUnit === "Micrometer"){
        result = fromValue * 25400;
      }
  
       //convert Yard into following units 
       if (fromUnit === "Yard" && toUnit === "kilometer") {
        result = fromValue / 1093.613;
      } else if (fromUnit === "Yard" && toUnit === "meter") {
        result = fromValue / 1.09361 ;
      } else if(fromUnit === "Yard" && toUnit === "Centimeter"){
        result = fromValue * 91.44;
      }
      else if(fromUnit === "Yard" && toUnit === "Nautical-miles"){
        result = fromValue / 2025.3718;
      }
      else if(fromUnit === "Yard" && toUnit === "Nanometer"){
        result = fromValue * 914400000;
      }
      else if(fromUnit === "Yard" && toUnit === "Inches"){
        result = fromValue * 36;
      }
      else if(fromUnit === "Yard" && toUnit === "Yard"){
        result = fromValue ;
      }
      else if(fromUnit === "Yard" && toUnit === "Miles"){
        result = fromValue / 1760;
      }
      else if(fromUnit === "Yard" && toUnit === "Millimeter"){
        result = fromValue * 914.4;
      }
      else if(fromUnit === "Yard" && toUnit === "Feet"){
        result = fromValue * 3;
      }
      else if(fromUnit === "Yard" && toUnit === "Micrometer"){
        result = fromValue * 914400;
      }
      //convert Miles into following units 
       if (fromUnit === "Miles" && toUnit === "kilometer") {
        result = fromValue * 1.609344;
      } else if (fromUnit === "Miles" && toUnit === "meter") {
        result = fromValue * 1609.344;
      } else if(fromUnit === "Miles" && toUnit === "Centimeter"){
        result = fromValue * 160934.4;
      }
      else if(fromUnit === "Miles" && toUnit === "Nautical-miles"){
        result = fromValue / 1.150779;
      }
      else if(fromUnit === "Miles" && toUnit === "Nanometer"){
        result = fromValue / 1609344000000;
      }
      else if(fromUnit === "Miles" && toUnit === "Inches"){
        result = fromValue * 63360;
      }
      else if(fromUnit === "Miles" && toUnit === "Yard"){
        result = fromValue * 1760;
      }
      else if(fromUnit === "Miles" && toUnit === "Miles"){
        result = fromValue ;
      }
      else if(fromUnit === "Miles" && toUnit === "Millimeter"){
        result = fromValue * 1609344;
      }
      else if(fromUnit === "Miles" && toUnit === "Feet"){
        result = fromValue * 5280;
      }
      else if(fromUnit === "Miles" && toUnit === "Micrometer"){
        result = fromValue * 1609344000;
      }
       //convert Millimeter into following units 
       if (fromUnit === "Millimeter" && toUnit === "kilometer") {
        result = fromValue / 1000000;
      } else if (fromUnit === "Millimeter" && toUnit === "meter") {
        result = fromValue / 1000;
      } else if(fromUnit === "Millimeter" && toUnit === "Centimeter"){
        result = fromValue / 10;
      }
      else if(fromUnit === "Millimeter" && toUnit === "Nautical-miles"){
        result = fromValue / 1852000;
      }
      else if(fromUnit === "Millimeter" && toUnit === "Nanometer"){
        result = fromValue * 1000000;
      }
      else if(fromUnit === "Millimeter" && toUnit === "Inches"){
        result = fromValue / 25.4;
      }
      else if(fromUnit === "Millimeter" && toUnit === "Yard"){
        result = fromValue / 914.4;
      }
      else if(fromUnit === "Millimeter" && toUnit === "Miles"){
        result = fromValue / 1609344;
      }
      else if(fromUnit === "Millimeter" && toUnit === "Millimeter"){
        result = fromValue ;
      }
      else if(fromUnit === "Millimeter" && toUnit === "Feet"){
        result = fromValue / 304.8;
      }
      else if(fromUnit === "Millimeter" && toUnit === "Micrometer"){
        result = fromValue * 1000;
      }
       //convert Feet into following units 
       if (fromUnit === "Feet" && toUnit === "kilometer") {
        result = fromValue / 3280.839895;
      } else if (fromUnit === "Feet" && toUnit === "meter") {
        result = fromValue / 3.280839895;
      } else if(fromUnit === "Feet" && toUnit === "Centimeter"){
        result = fromValue * 30.48;
      }
      else if(fromUnit === "Feet" && toUnit === "Nautical-miles"){
        result = fromValue / 6076.115485;
      }
      else if(fromUnit === "Feet" && toUnit === "Nanometer"){
        result = fromValue * 304800000;
      }
      else if(fromUnit === "Feet" && toUnit === "Inches"){
        result = fromValue * 12;
      }
      else if(fromUnit === "Feet" && toUnit === "Yard"){
        result = fromValue / 3;
      }
      else if(fromUnit === "Feet" && toUnit === "Miles"){
        result = fromValue / 5280;
      }
      else if(fromUnit === "Feet" && toUnit === "Millimeter"){
        result = fromValue * 304.8;
      }
      else if(fromUnit === "Feet" && toUnit === "Feet"){
        result = fromValue ;
      }
      else if(fromUnit === "Feet" && toUnit === "Micrometer"){
        result = fromValue * 304800;
      }
      
       //convert Micrometer into following units 
      if (fromUnit === "Micrometer" && toUnit === "kilometer") {
        result = fromValue / 1000000000;
      } else if (fromUnit === "Micrometer" && toUnit === "meter") {
        result = fromValue / 1000000;
      } else if(fromUnit === "Micrometer" && toUnit === "Centimeter"){
        result = fromValue / 10000;
      }
      else if(fromUnit === "Micrometer" && toUnit === "Nautical-miles"){
        result = fromValue / 1852000000;
      }
      else if(fromUnit === "Micrometer" && toUnit === "Nanometer"){
        result = fromValue / 1000;
      }
      else if(fromUnit === "Micrometer" && toUnit === "Inches"){
        result = fromValue / 25400;
      }
      else if(fromUnit === "Micrometer" && toUnit === "Yard"){
        result = fromValue / 914400;
      }
      else if(fromUnit === "Micrometer" && toUnit === "Miles"){
        result = fromValue / 1609344000;
      }
      else if(fromUnit === "Micrometer" && toUnit === "Millimeter"){
        result = fromValue * 1000;
      }
      else if(fromUnit === "Micrometer" && toUnit === "Feet"){
        result = fromValue / 304800;
      }
      else if(fromUnit === "Micrometer" && toUnit === "Micrometer"){
        result = fromValue ;
      }
      } else if (type === "weight") {
        // perform weight conversion
      //convert Tonnes into following units 
  
      if (fromUnit === "Grams" && toUnit === "Kilograms") {
        result = fromValue / 1000;
      } else if (fromUnit === "Grams" && toUnit === "Tonnes") {
        result = fromValue / 1000000;
      } else if(fromUnit === "Grams" && toUnit === "Stones"){
        result = fromValue / 6350.29318;
      }
      else if(fromUnit === "Grams" && toUnit === "Milligrams"){
        result = fromValue * 1000;
      }
      else if(fromUnit === "Grams" && toUnit === "Ounces"){
        result = fromValue * 28.349523125;
      }
      else if(fromUnit === "Grams" && toUnit === "Pounds"){
        result = fromValue / 453.59243;
      }
      else if(fromUnit === "Grams" && toUnit === "Long-Tons"){
        result = fromValue / 1016047.0431;
      }
      
      else if(fromUnit === "Grams" && toUnit === "Short-Tons"){
        result = fromValue / 907184.7;
      }
      else if(fromUnit === "Grams" && toUnit === "Micrograms"){
        result = fromValue * 1000000;
      }
      else if(fromUnit === "Grams" && toUnit === "Grams"){
        result = fromValue ;
      }
              // Kilograms 
       if (fromUnit === "Kilograms" && toUnit === "Grams") {
        result = fromValue * 1000;
      } else if (fromUnit === "Kilograms" && toUnit === "Tonnes") {
        result = fromValue / 1000;
      } else if(fromUnit === "Kilograms" && toUnit === "Kilograms"){
        result = fromValue;
      }
      else if(fromUnit === "Kilograms" && toUnit === "Stones"){
        result = fromValue / 6.35029318;
      }
      else if(fromUnit === "Kilograms" && toUnit === "Milligrams"){
        result = fromValue * 1000000;
      }
      else if(fromUnit === "Kilograms" && toUnit === "Ounces"){
        result = fromValue * 35.273961;
      }
      else if(fromUnit === "Kilograms" && toUnit === "Pounds"){
        result = fromValue * 2.2046223;
      }
      else if(fromUnit === "Kilograms" && toUnit === "Long-Tons"){
        result = fromValue / 1016.0470;
      }
     
      else if(fromUnit === "Kilograms" && toUnit === "Short-Tons"){
        result = fromValue / 907.1847;
      }
      else if(fromUnit === "Kilograms" && toUnit === "Micrograms"){
        result = fromValue * 1000000000;
      }
      
  //convert Tonnes into following units 
      if (fromUnit === "Tonnes" && toUnit === "Kilograms") {
        result = fromValue * 1000;
      } else if (fromUnit === "Tonnes" && toUnit === "Grams") {
        result = fromValue / 1000000;
      } else if(fromUnit === "Tonnes" && toUnit === "Tonnes"){
        result = fromValue;
      }
      else if(fromUnit === "Tonnes" && toUnit === "Stones"){
        result = fromValue * 157.4730;
      }
      else if(fromUnit === "Tonnes" && toUnit === "Milligrams"){
        result = fromValue * 1000000000;
      }
      else if(fromUnit === "Tonnes" && toUnit === "Ounces"){
        result = fromValue * 35273.96194;
      }
      else if(fromUnit === "Tonnes" && toUnit === "Pounds"){
        result = fromValue * 2204.6223;
      }
      else if(fromUnit === "Tonnes" && toUnit === "Long-Tons"){
        result = fromValue / 1.016047043;
      }
     
      else if(fromUnit === "Tonnes" && toUnit === "Short-Tons"){
        result = fromValue * 1.1023113595;
      }
      else if(fromUnit === "Tonnes" && toUnit === "Micrograms"){
        result = fromValue * 1000000000000;
      }
     
     
      //convert Stones into following units 
     if (fromUnit === "Stones" && toUnit === "Kilograms") {
        result = fromValue *6.35029318;
      } else if (fromUnit === "Stones" && toUnit === "Grams") {
        result = fromValue * 6350.29318;
      } else if(fromUnit === "Stones" && toUnit === "Tonnes"){
        result = fromValue / 157.47304 ;
      }
      else if(fromUnit === "Stones" && toUnit === "Stones"){
        result = fromValue ;
      }
      else if(fromUnit === "Stones" && toUnit === "Milligrams"){
        result = fromValue * 6350293.18;
      }
      else if(fromUnit === "Stones" && toUnit === "Ounces"){
        result = fromValue * 224;
      }
      else if(fromUnit === "Stones" && toUnit === "Pounds"){
        result = fromValue * 14;
      }
      else if(fromUnit === "Stones" && toUnit === "Long-Tons"){
        result = fromValue / 160;
      }
      
      else if(fromUnit === "Stones" && toUnit === "Short-Tons"){
        result = fromValue / 142.8571366;
      }
      else if(fromUnit === "Stones" && toUnit === "Micrograms"){
        result = fromValue * 6350293180;
      }
  
     //convert Milligrams into following units
   
     if (fromUnit === "Milligrams" && toUnit === "Kilograms") {
        result = fromValue / 1000000;
      } else if (fromUnit === "Milligrams" && toUnit === "Grams") {
        result = fromValue / 1000;
      } else if(fromUnit === "Milligrams" && toUnit === "Tonnes"){
        result = fromValue / 1000000000;
      }
      else if(fromUnit === "Milligrams" && toUnit === "Stones"){
        result = fromValue / 6350293.18;
      }
      else if(fromUnit === "Milligrams" && toUnit === "Milligrams"){
        result = fromValue ;
      }
      else if(fromUnit === "Milligrams" && toUnit === "Ounces"){
        result = fromValue / 28349.523125;
      }
      else if(fromUnit === "Milligrams" && toUnit === "Pounds"){
        result = fromValue / 453592.43;
      }
      else if(fromUnit === "Milligrams" && toUnit === "Long-Tons"){
        result = fromValue / 1016046000;
      }
      
      else if(fromUnit === "Milligrams" && toUnit === "Short-Tons"){
        result = fromValue / 907184700;
  
      }
      else if(fromUnit === "Milligrams" && toUnit === "Micrograms"){
        result = fromValue * 1000;
      }
  
  
      //convert Ounces into following units 
         if (fromUnit === "Ounces" && toUnit === "Kilograms") {
        result = fromValue / 35.273961;
      } else if (fromUnit === "Ounces" && toUnit === "Grams") {
        result = fromValue * 28.349523125;
      } else if(fromUnit === "Ounces" && toUnit === "Tonnes"){
        result = fromValue / 35273.961;
      }
      else if(fromUnit === "Ounces" && toUnit === "Stones"){
        result = fromValue / 224;
      }
      else if(fromUnit === "Ounces" && toUnit === "Milligrams"){
        result = fromValue * 28349.5231;
      }
      else if(fromUnit === "Ounces" && toUnit === "Ounces"){
        result = fromValue ;
      }
      else if(fromUnit === "Ounces" && toUnit === "Pounds"){
        result = fromValue / 16;
      }
      else if(fromUnit === "Ounces" && toUnit === "Long-Tons"){
        result = fromValue / 35840;
      }
      
      else if(fromUnit === "Ounces" && toUnit === "Short-Tons"){
        result = fromValue / 32000;
      }
      else if(fromUnit === "Ounces" && toUnit === "Micrograms"){
        result = fromValue * 28349523.12;
      }
  
       //convert Pounds into following units 
       if (fromUnit === "Pounds" && toUnit === "Kilograms") {
        result = fromValue / 2.204622330;
      } else if (fromUnit === "Pounds" && toUnit === "Grams") {
        result = fromValue* 453.592 ;
      } else if(fromUnit === "Pounds" && toUnit === "Tonnes"){
        result = fromValue / 2204.622330;
      }
      else if(fromUnit === "Pounds" && toUnit === "Stones"){
        result = fromValue / 14;
      }
      else if(fromUnit === "Pounds" && toUnit === "Milligrams"){
        result = fromValue * 453592.43;
      }
      else if(fromUnit === "Pounds" && toUnit === "Ounces"){
        result = fromValue * 16;
      }
      else if(fromUnit === "Pounds" && toUnit === "Pounds"){
        result = fromValue ;
      }
      else if(fromUnit === "Pounds" && toUnit === "Long-Tons"){
        result = fromValue / 2240;
      }
     
      else if(fromUnit === "Pounds" && toUnit === "Short-Tons"){
        result = fromValue * 2000;
      }
      else if(fromUnit === "Pounds" && toUnit === "Micrograms"){
        result = fromValue * 453592430;
      }
  
      //convert Long-Tons into following units
   
       if (fromUnit === "Long-Tons" && toUnit === "Kilograms") {
        result = fromValue * 1016.047043;
      } else if (fromUnit === "Long-Tons" && toUnit === "Grams") {
        result = fromValue * 1016047.0431;
      } else if(fromUnit === "Long-Tons" && toUnit === "Tonnes"){
        result = fromValue * 1.016047043;
      }
      else if(fromUnit === "Long-Tons" && toUnit === "Stones"){
        result = fromValue * 160;
      }
      else if(fromUnit === "Long-Tons" && toUnit === "Milligrams"){
        result = fromValue * 1016047043.1999;
      }
      else if(fromUnit === "Long-Tons" && toUnit === "Ounces"){
        result = fromValue * 35840;
      }
      else if(fromUnit === "Long-Tons" && toUnit === "Pounds"){
        result = fromValue * 2240;
      }
      else if(fromUnit === "Long-Tons" && toUnit === "Long-Tons"){
        result = fromValue ;
      }
  
      else if(fromUnit === "Long-Tons" && toUnit === "Short-Tons"){
        result = fromValue * 1.12000019753;
      }
      else if(fromUnit === "Long-Tons" && toUnit === "Micrograms"){
        result = fromValue * 1016047043199.9;
      }
      
       //convert Short-Tons into following units 
       if (fromUnit === "Short-Tons" && toUnit === "Kilograms") {
        result = fromValue * 907.1847;
      } else if (fromUnit === "Short-Tons" && toUnit === "Grams") {
        result = fromValue * 907184.7;
      } else if(fromUnit === "Short-Tons" && toUnit === "Tonnes"){
        result = fromValue / 1.102311359;
      }
      else if(fromUnit === "Short-Tons" && toUnit === "Stones"){
        result = fromValue * 142.8571;
      }
      else if(fromUnit === "Short-Tons" && toUnit === "Milligrams"){
        result = fromValue * 907184700;
      }
      else if(fromUnit === "Short-Tons" && toUnit === "Ounces"){
        result = fromValue * 32000;
      }
      else if(fromUnit === "Short-Tons" && toUnit === "Pounds"){
        result = fromValue * 2000;
      }
      else if(fromUnit === "Short-Tons" && toUnit === "Long-Tons"){
        result = fromValue / 1.1200001975;
      }
      
      else if(fromUnit === "Short-Tons" && toUnit === "Short-Tons"){
        result = fromValue ;
      }
      else if(fromUnit === "Short-Tons" && toUnit === "Micrograms"){
        result = fromValue * 907184700000;
      }
      
       //convert Micrograms into following units 
  
      if (fromUnit === "Micrograms" && toUnit === "Kilograms") {
        result = fromValue / 1000000000;
      } else if (fromUnit === "Micrograms" && toUnit === "Grams") {
        result = fromValue / 1000000;
      } else if(fromUnit === "Micrograms" && toUnit === "Tonnes"){
        result = fromValue / 1000000000000;
      }
      else if(fromUnit === "Micrograms" && toUnit === "Stones"){
        result = fromValue / 6350293180;
      }
      else if(fromUnit === "Micrograms" && toUnit === "Milligrams"){
        result = fromValue / 1000;
      }
      else if(fromUnit === "Micrograms" && toUnit === "Ounces"){
        result = fromValue / 28349523.125;
      }
      else if(fromUnit === "Micrograms" && toUnit === "Pounds"){
        result = fromValue / 453592430;
      }
      else if(fromUnit === "Micrograms" && toUnit === "Long-Tons"){
        result = fromValue / 1016047043199.982;
      }
      
      else if(fromUnit === "Micrograms" && toUnit === "Short-Tons"){
        result = fromValue / 907184700000;
      }
      else if(fromUnit === "Micrograms" && toUnit === "Micrograms"){
        result = fromValue ;
  }
      } else if (type === "area") {
        // perform area conversion
        if (fromUnit === "square feet" && toUnit === "square meters") {
          result = fromValue * 0.092903;
        } else if (fromUnit === "square meters" && toUnit === "square feet") {
          result = fromValue / 0.092903;
        }
      } else if( type==="Tempreture"){
              // perform Tempreture  conversion 
  
  
  //convert Celsius into following units 
  
   if (fromUnit === "Celsius" &&  toUnit === "Fahrenheit") {
        result = fromValue * 1.8 + 32;
      } else if (fromUnit === "Celsius" && toUnit === "Rankine") {
        result = fromValue * 1.8 + 491.67;
      } else if(fromUnit === "Celsius" && toUnit === "Kelvins"){
        result = fromValue + 273.15;
     } else if(fromUnit === "Celsius" && toUnit === "Celsius"){
        result = fromValue ;
     }
  
  //convert Fahrenheit into following units 
  
   if (fromUnit === "Fahrenheit" &&  toUnit === "Fahrenheit") {
        result = fromValue ;
      } else if (fromUnit === "Fahrenheit" && toUnit === "Rankine") {
        result = fromValue + 459.67;
      } else if(fromUnit === "Fahrenheit" && toUnit === "Kelvins"){
      result = (fromValue - 32) * 5/9  + 273.15;
     } else if(fromUnit === "Fahrenheit" && toUnit === "Celsius"){
         result = (fromValue - 32) * 5/9 ;
     }
  
  //convert Rankine into following units 
  
   if (fromUnit === "Rankine" &&  toUnit === "Fahrenheit") {
        result = fromValue - 459.67 ;
      } else if (fromUnit === "Rankine" && toUnit === "Rankine") {
        result = fromValue ;
      } else if(fromUnit === "Rankine" && toUnit === "Kelvins"){
      result = fromValue  * 5/9  ;
     } else if(fromUnit === "Rankine" && toUnit === "Celsius"){
         result = (fromValue - 491.67) * 5/9 ;
     }
  
  //convert Kelvins into following units 
  
   if (fromUnit === "Kelvins" &&  toUnit === "Fahrenheit") {
      result = (fromValue -273.15) * 9/5  +32 ;
      } else if (fromUnit === "Kelvins" && toUnit === "Rankine") {
        result = fromValue * 1.8;
      } else if(fromUnit === "Kelvins" && toUnit === "Kelvins"){
      result = fromValue   ;
     } else if(fromUnit === "Kelvins" && toUnit === "Celsius"){
         result = fromValue - 273.15 ;
     }
          }
    }
  </script>
  
  <div>
    <label for="type-select">Unit Type:</label>
    <select id="type-select" bind:value={type}>
      <option value="length">Length</option>
      <option value="weight">Weight</option>
           <option value="Tempreture">Tempreture</option>
      <option value="area">Area</option>
    </select>
  </div>
  
  <div>
    <label for="from-value">Value:</label>
    <input type="number" id="from-value" bind:value={fromValue}>
  </div>
  
  <div>
    <label for="from-unit">Unit:</label>
    <select id="from-unit" bind:value={fromUnit}>
      {#if type === "length"}
           <option value="meter">Meter</option>
       <option value="kilometer">kiloMeter</option>
        <option value="Centimeter">CentiMeter</option>
        <option value="Nautical-miles">Nautical Miles</option>
        <option value="Nanometer">Nanometer</option>
        <option value="Inches">Inches</option>
        <option value="Yard">Yard</option>
        <option value="Miles">Miles</option>
        <option value="Millimeter">Millimeter</option>
        <option value="Micrometer">Micrometer</option>
        <option value="Feet">Feet</option>
      {:else if type === "weight"}
         <option value="Grams">Grams</option>
       <option value="Kilograms">Kilograms</option>
        <option value="Tonnes">Tonnes</option>
        <option value="Stones">Stones</option>
        <option value="Milligrams">Milligrams</option>
        <option value="Ounces">Ounces</option>
        <option value="Pounds">Pounds</option>
        <option value="Long-Tons">Long-Tons</option>
        <option value="Short-Tons">Short-Tons</option>
        <option value="Micrograms">Micrograms</option>
      {:else if type === "Tempreture"}
        <option value="Celsius">Celsius</option>
        <option value="Fahrenheit">Fahrenheit</option>
           <option value="Fahrenheit">Fahrenheit</option>
           <option value="Rankine">Rankine</option>
           <option value="Kelvins">Kelvins</option>
           {:else if type === "area"}
            <option value="square feet">Square Feet</option>
        <option value="square meters">Square Meters</option>
      {/if}
    </select>
  </div>
  
  <div>
    <label for="to-unit">Convert to:</label>
    <select id="to-unit" bind:value={toUnit}>
      {#if type === "length"}
           <option value="meter">Meter</option>
       <option value="kilometer">kiloMeter</option>
        <option value="Centimeter">CentiMeter</option>
        <option value="Nautical-miles">Nautical Miles</option>
        <option value="Nanometer">Nanometer</option>
        <option value="Inches">Inches</option>
        <option value="Yard">Yard</option>
        <option value="Miles">Miles</option>
        <option value="Millimeter">Millimeter</option>
        <option value="Micrometer">Micrometer</option>
        <option value="Feet">Feet</option>
      {:else if type === "weight"}
       <option value="Grams">Grams</option>
       <option value="Kilograms">Kilograms</option>
        <option value="Tonnes">Tonnes</option>
        <option value="Stones">Stones</option>
        <option value="Milligrams">Milligrams</option>
        <option value="Ounces">Ounces</option>
        <option value="Pounds">Pounds</option>
        <option value="Long-Tons">Long-Tons</option>
        <option value="Short-Tons">Short-Tons</option>
        <option value="Micrograms">Micrograms</option>
      {:else if type === "Tempreture"}
      <option value="Celsius">Celsius</option>
        <option value="Fahrenheit">Fahrenheit</option>
           <option value="Fahrenheit">Fahrenheit</option>
           <option value="Rankine">Rankine</option>
           <option value="Kelvins">Kelvins</option>
           {:else if type === "area"}
        <option value="square feet">Square Feet</option>
        <option value="square meters">Square Meters</option>
      {/if}
    </select>
  </div>
  
  <button on:click={convert}>Convert</button>
  
  <div>
    Result: {result} {toUnit}
  </div>
  
  