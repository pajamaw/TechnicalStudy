Data types (in ruby)
  - booleans
  - symbols (specific to ruby symbols can be through of as attributes that'd you input as a column in your database e.g. :age)
  - numbers
    divided into
        Fixnum
        Float
        Bignum
  - strings
  - Arrays
  - hashes

Duck Typing - "An object is defined by what it can do, not by what ist is. It's because in Ruby we're less concered with the class of an object and more concered with what methods are called on it and what opersations can be performed on it....if an object walks like a duck and talks like a duck...its probably a duck! --> this is opposed to "Structural typing...which is concered more about the actual structure or definiition and nominataive systems which are concerned more strictly about the naming and explicit declarations of objects "

Programming Language vs. Scripting language -
  Scripting languages are interpreted rather than compiled...they mediate between programs to change data as opposed to programming lanaguages which actually transform Data

  ooP - lanaguage model is organized around objects which communicate with each other as opposed to being around "actions"

  Basic Bitwise Operations - these are &	The AND operator
  |	The OR operator
  ^	The XOR operator
  ~	The NOT (complement) operator
  «	The left shift operator
  »	The right shift operator
  whoahhh never knew this!
  (a = 18).to_s(2)     #=> "10010"
  (b = 20).to_s(2)     #=> "10100"
  (a & b).to_s(2)      #=> "10000"
  lots of cool things with this
  https://calleerlandsson.com/2014/02/06/rubys-bitwise-operators/
  so the to_s(number) that number equals the base, so you do 2 to mean Binary

String Operations
Arrays - datatype
Linked Lists -
  http://matt.weppler.me/2013/08/14/implementing-a-linked-list-in-ruby.html

Singly Linked
Doubly Linked
Circular Linked
Queues - FIfo
Stacks -LIFO
  https://rubymonk.com/learning/books/4-ruby-primer-ascent/chapters/33-advanced-arrays/lessons/86-stacks-and-queues#solution4117
Heaps
  heaps can be stored as arrays, go top to bottom left to right....but it has to be stored via the condition that the "max heap, is always a t the top. there cannot be larger connected nodes to smaller nodes"
  https://www.sitepoint.com/heap-data-structure-ruby/
Trees
  http://zvkemp.github.io/blog/2014/04/25/binary-search-trees-in-ruby/
Binary Trees
  http://zvkemp.github.io/blog/2014/04/25/binary-search-trees-in-ruby/
Binary Search Trees
Tries
Self Balancing Trees
Traversing Trees
Breadth First Search - BFS
Depth First Search - DFS
Preorder, Inorder, Postorder
Graphs
Dijkstra's Algorithm / A* Search
Hash Maps
Handling Collisions
Sorting algorithms
Insertion
Selection
Merge
Quick
Time Complexities
GENERAL GUIDES
Sorting Algorithms
Big-O Cheat Sheet
Data Structures and Algorithms Overview
Algorithm Implementations
Top 10 Algorithms for Coding Interviews
PROBLEM SETS
Data Structures Questions
Fit Coding
Google CodeJam Practice Questions
ONLINE JUDGING SYSTEMS
LeetCode Online Judge
HackerRank Online Judge
Project Euler
MOCK INTERVIEWS
Pramp
Careercup
Gainlo
Impact Interview
Interview Cake
ACTUAL INTERVIEW QUESTIONS
Flatiron School Student Interview Questions
Technical Interview Questions
BOOKS
Algorithms, 4th edition, by Robert Sedgewick and Kevin Wayne
Introduction to Algorithms, 3rd Edition, by Thomas H. Cormen, Charles E. Leiserson, Ronald L. Rivest, and Clifford Stein (also referred as CLRS)
Think Complexity, by Allen Downey
Problems on Algorithms, 2nd edition, by Ian Parberry and William Gasarch
Data Structures and Algorithms in Java
Cracking the Coding Interview, 6th edition, by Gayle Laakmann McDowell

def get_all(array)
array.sort!
  array.each do |num|
    array.delete(num)
    a = array.inject(:*)
    puts a
    array.unshift(num)
    array.sort!
  end
end
