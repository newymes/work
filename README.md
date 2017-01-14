# work
For problems 1 through 4, explain why the code as shown is almost certainly not what the programmer intended, and how it should be fixed to work the way the programmer probably had in mind.
1. (10 pts) What is wrong with the following program and how should it be fixed?
1  public class MyClassA {
2    int v = 12;
3 
4    public MyClassA (int pV) {
5      v = pV;
6    } 
7 
8    public static void main (String args []) {
9      MyClassA m = new MyClassA ();
10   } // end main
11 } // end class MyClassA
2. (10 pts) What is wrong with the following program and how should it be fixed?
1  public class MyClassB {
2    int v = 12;
3 
4    public void MyClassB (int pV) {
5      v = pV;
6    } 
7 
8    public static void main (String args []) {
9      MyClassB m = new MyClassB (23);
10   } // end main
11 } // end class MyClassB
3. (10 pts) What is wrong with the following program and how should it be fixed?
1   public class MyClassD {
2     public static void main (String args []) {
3       MyClassC m = new MyClassC (23);
4     } // end main
5   } // end class MyClassD
6 
7   class MyClassC {
8     int v = 12;
9 
10    public MyClassC (int pV) {
11      int v = pV;
12    } 
13 
14  } // end class MyClassC

4. (10 pts) What is wrong with the following program and how should it be fixed?
1   public class MyClassE {
2     public static void main (String args []) {
3       MyClassF m = new MyClassF (23);
4     } // end main
5   } // end class MyClassE
6 
7   class MyClassF {
8     int v = 12;
9 
10    private MyClassF (int pV) {
11      v = pV;
12    } 
13 
14  } // end class MyClassF
5. (10 pts) Given all the problems identified in problems 1 through 4, explain in detail why the following code works, ie, compiles without errors or warnings.
1  public class MyClassG {
2    public static void main (String args []) {
3      MyClassH m = new MyClassH (23, true);
4    } // end main
5  } // end class MyClassG
6 
7  class MyClassH {
8    int v = 12;
9 
10   public MyClassH (int x, boolean b) {
11     this (x);
12   } 
13 
14   private MyClassH (int pV) {
15     v = pV;
16   } 
17 
18 } // end class MyClassH
6. (10 pts) Explain why the following class hierarchy is not reasonable:
•	DefenseDepartment
o	General
	Private
Answer:
Because the Private organization is part of the Department of the Defense
7. (10 pts) Give at least one example of a reasonable field for each of the following classes in the following class hierarchy. Be sure that the field is at the right level in the hierarchy.
•	Vehicle
o	Car
o	Airplane
	Passenger
	Fighter
	Bomber
o	SpaceShip
8. (10 pts) Give at least one example of a reasonable method for each of the following classes in the following class hierarchy. Be sure that the method  is at the right level in the hierarchy. Constructors, getters and setters don't count for this problem.
•	Vehicle
o	Car
o	Airplane
	Passenger
	Fighter
	Bomber
o	SpaceShip
9. (10 pts) Are a Private and a Platoon in an encapsulation or an inheritance relationship? Explain

10. (10 pts) Present reasonable parent and child classes for the class Tree (the biological kind). Give a short explanation for why the classes you are proposing are in good parent-child relationships.
