# Memory Management

### How is it handeled?

#### **Kotlin**
  - 
  
#### **Swift**
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Swift handles memory management through a proccess called ARC or Automatic Reference Counting.  This proccess allows for easy memory management for the programmer because Swift will do deallocates and allocates for you.  Swift will not deallocate an object unless it leaves the scope that it is contained in.

**For Example:**

let test = Test(number: 1)   // Will not be deallocated until main program is over

while(counter!= 2){

&nbsp;&nbsp;let test = Test(number: 1)  // Will be deallocated after the while loop is over

}


Objects in swift go through a 5 stage process after allocation.  The 5 steps are:

&nbsp;&nbsp; -Allocation (memory taken from stack or heap)

&nbsp;&nbsp; -Initialization (init code runs)

&nbsp;&nbsp; -Usage (the object is used)

&nbsp;&nbsp; -Deinitialization (deinit code runs)

&nbsp;&nbsp; -Deallocation (memory returned to stack or heap)
