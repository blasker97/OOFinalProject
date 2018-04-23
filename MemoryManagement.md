# Memory Management

#### **Kotlin**
  - 
  
## **Swift**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Swift handles memory management through a proccess called ARC or Automatic Reference Counting.  This proccess allows for easy memory management for the programmer because Swift will do deallocates and allocates for you.  Swift will not deallocate an object unless it leaves the scope that it is contained in.

**For Example:**
```swift
let test = Test(number: 1)   // Will not be deallocated until main program is over

vs

while(counter!= 2){
  let test = Test(number: 1)  // Will be deallocated after the while loop is over
}
```
#### **The Proccess**
Objects in swift go through a 5 stage process after allocation.  The 5 steps are:

&nbsp;&nbsp; -Allocation (memory taken from stack or heap)

&nbsp;&nbsp; -Initialization (init code runs)

&nbsp;&nbsp; -Usage (the object is used)

&nbsp;&nbsp; -Deinitialization (deinit code runs)

&nbsp;&nbsp; -Deallocation (memory returned to stack or heap)

#### **The good**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The advantages of the ARC cycle is the developer does not have to worry about memory leaks because as soon as something leaves its scope the reference count will be updated for the current scope of the program.  With this as soon as the reference counter hits 0 Swift will automatically deinitalize the object and return the memory back to the stack or heap.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Swifts automatic reference counting allows for easy garabage collection because as soon as the reference count hits 0 it will be marked as garbage and the memory will be returned.

#### **The Bad**

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
