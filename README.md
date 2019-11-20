# Text-Difference-Finder
Problem Statement:
    In a public app, where one person is writing something(say a solution to some problem or simple English sentences) for other people, he/she can make mistakes. The FINDER can fix that writings or may edit them. For Example, One person write "The breakfast I had tooday was aweesome". Then, the FINDER will be able to identify that there are spellings  mistakes in that sentence. So it's going to correct it as , "The breakfast I had today was awesome". There are many ways to solve this problem i.e. , writing the complete sentence again, just writing the corrected words say "today" and "awesome" or just remove an 'o' from "tooday" and removing an 'e' after 'w' in "aweesome". The FINDER will find the difference between the correct words and the mistaken ones. After comparison the correct words will be replaces by the mistaken words. The comparison can be of words or of characters. 
Let’s see another Example:
Original Sentence: I am waiting.
Fixed: I’ve been waiting.
LCS = I  waiting.
*For Checking the removed part from Original String we compare the LCS with Original String.
“I am waiting.”
*For checking the added or edited part, we compare the LCS with Fixed String.
“I’ve been waiting.”
  That’s how it is going to work. The Mistakes will be highlighted and we’ll know what changes have been made to make our stuff right.
We are going to use the Dynamic Programming Approach and the concept of Longest common sub-sequence for solving this problem. This will reduce our time complexity to O(l1*l2) from 2(l1*l2)  , where l1 represents the length of first sentence and l2 represents the length of second sentence.
