# Exp No: 36  
## Circular Queue 

### AIM  
To write a Python program with a function to insert float values into a Circular Queue.

### ALGORITHM

1. Start  
2. Check if the Circular Queue is full  
   - If `size == max_size`, print `"Queue is full"` and exit the function  
3. If the queue is not full:  
   - Read the element to be inserted  
   - Convert it to float  
   - Insert the element at the `tail` position  
   - Update tail using: `tail = (tail + 1) % max_size` (circular increment)  
   - Increment `size` by 1  
4. End

---

### PROGRAM

```
Reg.No: 212222060182
Name: Preethika S

class Queue:
def init(self, size):
self.items = [0] * size
self.max_size = size
self.head, self.tail, self.size = 0, 0, 0
def enqueue(self, item):
if self.is_list_full():
print("Queue is full")
return
self.items[self.tail]=item
self.tail=(self.tail+1)%self.max_size
self.size+=1
def is_list_full(self):
if self.size==self.max_size:
return True
return False

def is_empty(self):
if self.size==0:
return True
return False

size=int(input())
queue=Queue(size)
str=float(input())
str1=float(input())
str2=float(input())
queue.enqueue(str)
queue.enqueue(str1)
queue.enqueue(str2)
print(queue.items)


```

### OUTPUT
![image](https://github.com/user-attachments/assets/b7557263-d767-4bcb-9cff-52bde1562619)

### RESULT
Thus , the given python program is implemented and executed sucessfully.
