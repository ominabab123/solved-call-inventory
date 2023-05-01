Download Link: https://assignmentchef.com/product/solved-call-inventory
<br>
Write a unit test for addInventory(). Call redSweater.addInventory() with parameter sweaterShipment. Print the shown error if the subsequent quantity is incorrect. Sample output for failed unit test given initial quantity is 10 and sweaterShipment is 50:

// ===== Code from file InventoryTag.java =====public class InventoryTag {private int quantityRemaining;

public InventoryTag() {quantityRemaining = 0;}

public int getQuantityRemaining() {return quantityRemaining;}

public void addInventory(int numItems) {if (numItems &gt; 10) {quantityRemaining = quantityRemaining + numItems;}return;}}// ===== end =====

// ===== Code from file CallInventoryTag.java =====public class CallInventoryTag {public static void main (String [] args) {InventoryTag redSweater = new InventoryTag();int sweaterShipment = 0;int sweaterInventoryBefore = 0;

sweaterInventoryBefore = redSweater.getQuantityRemaining();sweaterShipment = 25;

System.out.println(“Beginning tests.”);

// FIXME add unit test for addInventory

/* Your solution goes here */redSweater.addInventory(25);if(redSweater.getQuantityRemaining() != 25 ){System.out.println(“UNIT TEST FAILED: addInventory()”);}redSweater.addInventory(5);if(redSweater.getQuantityRemaining()!= 25){System.out.println(“UNIT TEST FAILED: addInventory()”);}

System.out.println(“Tests complete.”);

return;}}// ===== end =====

Once I run the test I always get stuck on the last one (with the X in front). Is there code I am missing in order to get the correct result?

Inventory is 0, shipment is 25. Testing that quantityRemaining was updated to 25.

Your value: 25

Testing with sweaterShipment of 25. addInventory updates quantityRemaining.

Your output: Beginning tests.

Tests complete.

? Inventory is 25, shipment is 5. Testing that quantityRemaining remains 25.

Expected value: 25

Your value: 50

Tests aborted.