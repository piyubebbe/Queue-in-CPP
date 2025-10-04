# Implementation of Queue in C++

**Aim:** To study and implement Queue in C++  
**Software:** Mingw C/C++ compiler, VS Code, online C++ compiler  

## Program 1

### Explanation with Theory of Code

**Queue Concept:**  
A queue is a linear data structure following the FIFO (First-In-First-Out) principle.

**Fixed Size:**  
The queue uses a static array of size 5 (`#define SIZE 5`).

**Initialization:**  
`start` and `end` are initialized to `-1` to indicate an empty queue.

**Enqueue Operation:**
- Checks for overflow (`end == SIZE - 1`).
- If queue is empty (`start == -1`), sets `start = 0`.
- Inserts element at `++end` position.

**Dequeue Operation:**
- Checks for underflow (`start == -1` || `start > end`).
- Removes element at `start` and increments `start`.

**Display Function:**
- Prints elements from `start` to `end`.
- Handles empty queue condition.

**Main Function:**  
Demonstrates enqueue, dequeue, and display operations.

---

### Algorithm

1. **Start**
2. Initialize queue with `start = -1`, `end = -1` and array of fixed size.
3. **Enqueue operation**: Check if queue is full, if not insert element at `end + 1`.
4. **Dequeue operation**: Check if queue is empty, if not remove element from `start`.
5. **Display operation**: Print elements from `start` to `end`.
6. In `main`: Perform enqueue, display, dequeue, and enqueue operations as required.
7. **Stop**

---

### Conclusion

The array-based queue implementation offers a simple yet effective way to manage data in a linear FIFO structure. By using fixed-size storage and two pointers (`start` and `end`), it efficiently handles insertion and deletion operations while maintaining order.  
Though limited by static size and lack of circular reuse, it serves as a foundational model for understanding queue behavior.  
This program demonstrates key operations—enqueue, dequeue, and display—along with overflow and underflow conditions, making it ideal for beginners.  
Overall, it reinforces core concepts of data structures and prepares learners for more advanced dynamic or circular queue implementations.
