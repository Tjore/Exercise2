# Mutex and Channel basics

### What is an atomic operation?
> An uninterruptable read/write operation. 

### What is a semaphore?
> It's a way to limit the number of consumers for a specific resource. A counter that only can increment or decrement.

### What is a mutex?
> Like a semaphore, but only has the values (0,1). Locks a resourse to a single user.

### What is the difference between a mutex and a binary semaphore?
> A mutex locks ownership to a single prosess, and others cant get to it while the owner has it. 
> Binary semaphore is simelar, but any process can come and increment/decrement the counter(binary has limit of 1).

### What is a critical section?
> A critical section is a bit of code where the program is vulnerable for disruption by other threads

### What is the difference between race conditions and data races?
 > A race condition is the possiblillity of things going wrong (originates from bad code), data races is when it goes wrong.
 > related to concurrensy errors.

### List some advantages of using message passing over lock-based synchronization primitives.
> Message passing can be queued, and worked through when there is time for it. This allows for asychronus programming.
> Removes some deadlock problems (example: Dining philosophers problem).

### List some advantages of using lock-based synchronization primitives over message passing.
> Writing/reading operations has to be locked to not jumble the data.
