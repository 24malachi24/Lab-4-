Lab 4 
// Class Ciruit Demo 
                    /**
 * A class to run tests on the Circuit class and subclasses
 * @author Horstman
 * @version 02/06/2014
 *  
 */
public class CircuitDemo
{ /**
method that implements tests for Circuit class and sublclasses
@param args - Not Used.
  */
   public static void main(String[] args)
   {
      Parallel circuit1 = new Parallel();
      circuit1.add(new Resistor(100));
      Serial circuit2 = new Serial();
      circuit2.add(new Resistor(100));
      circuit2.add(new Resistor(200));
      circuit1.add(circuit2);
      System.out.println("Combined resistance: " + circuit1.getResistance());
      System.out.println("Expected: 75.0");
   }
}

                                            Class Circuit
                                                 
    public class Circuit{
          
         public float getResistance(){
              return 0;
         
         }
    }
        
                                                    CLASS SERIAL 
       
      
     public class Serial extends Circuit{
          //Array list of type circuit. 
          ArrayList<Circuit> circuits  = new ArrayList<Circuit>;
          
          
          
          
            public float getResistance(){
            //This sum only needs to exist in this loop.
            float sum = 0;
            //for each loop 
             for (Circuit C : circuits ){
                  C;
            
             }
              return sum;
         
         }
     
     }
              
                
                
                
                
   
                    
                    
                    
           
                                            
                                            


                                        Class Resistor 
 
 public class Resistor extends Circuit{
 
    private float Resistance;
    
      public Resistor(float Resitance){
      //
      
      this.Resitance = Resitance;
      
      }   
      
      public float getResistance(){
      
         return float Resistance;
      }
 }
