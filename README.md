# ACID properties and BASE properties

ACID properties:-

Atomic: Everything in a transaction succeeds or the entire transaction is rolled back.
Consistent: A transaction cannot leave the database in an inconsistent state.
Isolated: Transactions cannot interfere with each other.
Durable: Completed transactions persist, even when servers restart etc.

BASE properties:-

Basic Availability
Soft-state
Eventual consistency

# paging and segmentation

Paging:-

Paging is a memory management technique in which process address space is broken into blocks of the same size called pages (size is power of 2, between 512 bytes and 8192 bytes). The size of the process is measured in the number of pages. Similarly, main memory is divided into small fixed-sized blocks of (physical) memory called frames and the size of a frame is kept the same as that of a page to have optimum utilization of the main memory and to avoid external fragmentation.

Similarly, main memory is divided into small fixed-sized blocks of (physical) memory called frames and the size of a frame is kept the same as that of a page to have optimum utilization of the main memory and to avoid external fragmentation.

Segmentation:-

Segmentation is a memory management technique in which each job is divided into several segments of different sizes, one for each module that contains pieces that perform related functions. Each segment is actually a different logical address space of the program. When a process is to be executed, its corresponding segmentation are loaded into non-contiguous memory though every segment is loaded into a contiguous block of available memory. Segmentation memory management works very similar to paging but here segments are of variable-length where as in paging pages are of fixed size.

A program segment contains the program's main function, utility functions, data structures, and so on. The operating system maintains a segment map table for every process and a list of free memory blocks along with segment numbers, their size and corresponding memory locations in main memory. For each segment, the table stores the starting address of the segment and the length of the segment. A reference to a memory location includes a value that identifies a segment and an offset.

# OOPS principles

There are 4 major principles that make an language Object Oriented. 
These are 

Encapsulation, 
Abstraction, 
Polymorphism, 
Inheritance.

These are also called as four pillars of Object Oriented Programming.

Encapsulation:-

Encapsulation is the mechanism of hiding of data implementation by restricting access to public methods. Instance variables are kept private and accessor methods are made public to achieve this.

Abstraction:-

Abstract means a concept or an Idea which is not associated with any particular instance. Using abstract class/Interface we express the intent of the class rather than the actual implementation. In a way, one class should not know the inner details of another in order to use it, just knowing the interfaces should be good enough.

Polymorphism:-

It means one name many forms. It is further of two types — static and dynamic. Static polymorphism is achieved using method overloading and dynamic polymorphism using method overriding. It is closely related to inheritance. We can write a code that works on the superclass, and it will work with any subclass type as well.

Inheritance:-

Inheritances expresses “is-a” and/or “has-a” relationship between two objects. Using Inheritance, In derived classes we can reuse the code of existing super classes.

# Happen when you write www.google.com in your web browser 

browser checks cache; if requested object is in cache and is fresh, skip to #9
browser asks OS for server's IP address
OS makes a DNS lookup and replies the IP address to the browser
browser opens a TCP connection to server (this step is much more complex with HTTPS)
browser sends the HTTP request through TCP connection
browser receives HTTP response and may close the TCP connection, or reuse it for another request
browser checks if the response is a redirect (3xx result status codes), authorization request (401), error (4xx and 5xx), etc.; these are handled differently from normal responses (2xx)
if cacheable, response is stored in cache
browser decodes response (e.g. if it's gzipped)
browser determines what to do with response (e.g. is it a HTML page, is it an image, is it a sound clip?)
browser renders response, or offers a download dialog for unrecognized types


# Which of the following condition is required for a deadlock to be possible
a) mutual exclusion

# Which one of the following is the deadlock avoidance algorithm?
a) banker's algorithm

# To avoid deadlock
b) resource allocation must be done only once

# A Process Control Block(PCB) does not contain which of the following?
c) Bootstrap program

# Which of the following is not the state of a process?
b) Old
