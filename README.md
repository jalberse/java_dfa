# Java DFA
An example of a DFA implemented in Java

## Intent

This is a tool to check that a DFA has been properly constructed by testing if, given a string, it provides the correct classification. It is meant to be used as a study aide by students studying DFA construction.

For example, we examine a motivating problem, "construct a DFA M such that L(M) = L where L is the set of all strings over {0,1} with exactly two occurances of the substring 01000111." Students may construct a DFA for such a language, but may have a hard time verifying its correctness. It is trivial to construct examples and counter-examples of words for L, so students may use this program and examples they come up with to ensure the correctness of their DFA, or to aide in its design.

Note that his program does NOT mathematically verify that L(M) = L. This problem is non-trivial. This program only verifies that a DFA M, given w, does or does not match the classification of w provided by the user.

## Input format

Input files should be .txt files containing the following lines:

```
Description
# of states
Input alphabet (e.g. abcd)
Comma separated list of accepting states (e.g. 0,1,3)
Starting state
Enumeration of transitions, one per line. e.g. T(0,a)->(1) is written 0,a,1
```
