# Java code for one to one character mapping.
The goal of this code is to determine whether a one-to-one character mapping exists from one string, s1, to another string,s2. For example, Given s1 = abc and s2 = bcd , print " true" into stdout since we can map each character in "abc" to a character in "bcd". Given s1 = foo and s2 = bar, print " false" since the character ‘o’ cannot map to two characters. But given s1 = bar and s2 = foo, print "true " since each character in "bar" can be mapped to a character in "foo".

There are two approaches to this problem as stated below:

# Approach1:-
When we do one-to-one character mapping based on indexing. For Example: if the input in string s1=foo and s2=aba then the output of the code should be false since o in string s1 cannot be mapped to two characters.

# Approach2:-
When we do one-to-one character mapping not based on indexing. For Example: if the input in string s1=foo and s2=aba then the output of the code should be true since o in string s1 can be mapped to 2 a's in string s2 and f can be mapped to b character in string s2.

I have implemented the code based on Approach2(To implement using Approach1 we only need a Hashmap and check if the character in string s1 is in Hashmap or not and if not then add and if it is present then simply check if the value of that key is equal to the character in string s2 if no then print false else at the end after all the iterations print true.)

Input for this program is two strings as command-line arguments and output is a corresponding message describing whether one-to-one character mapping exists between two strings. Java is used for implementation purpose and you can execute the program using "java main.java s1 s2" in command prompt.

Steps followed during implementations are as follows:

1.Count frequencies of characters in both strings

2.Build Max heap for frequencies of both strings

3.Iterate over frequencies

4.Turn the flag to False if the frequencies don't match

5.Print the Result based on flag value
