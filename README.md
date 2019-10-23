
# Introduction to Sets, continued

## Introduction

In this Module, you learned about the formal definition of sets, set operations, how to visualize set operations using Venn Diagrams, and how to define sets using Python. 

In this Appendix lesson, we dive a bit deeper into the mathematical notation used when referring to sets, we distinguish between subsets and proper subsets, and we define the inclusion/exclusion principle. 

## Objectives

You will be able to: 

* Describe the inclusion-exclusion principle


## What is a Set? 

In probability theory, a set is defined as a *well-defined collection of objects*. 

Mathematically, you can denote a set by $S$. If an element $x$ belongs to a set $S$, then you'd write $x \in S$. On the other hand, if $x$ does not belong to a set $S$, then you'd write $x\notin S$.

Thus, using the example used in the introduction to sets lesson, if $S$ is defined as the set of even numbers, then:

* If $x = 2$, $x\in S$.

* If $x = 9$, $x\notin S$.


## Subsets and Proper Subsets

Set $T$ is a subset of set $S$ if *every element* in set $T$ is also in set $S$. The mathematical notation for a subset is $T \subseteq S$. 

Typically, you'll be more interested in *proper subsets*. All proper subsets are subsets. The only difference between subsets and proper subsets is that a subset can technically be the entire set. In other words, if A = {1,2,3} and B = {1,2,3} A is subset of B. If C = {1,2} then C is both a subset and proper subset of A. C is also a subset and proper subset of B. The mathematical notation for proper subsets is : $ C \subset A $

**Example**: If S is the set of even numbers, set $T = \{2, 6, 22\}$ is a proper subset of $S$. Formally, you can write this as $T \subset S$. $T \subseteq S$ is also correct in this case!


## Inclusion-Exclusion Principle

Imagine you have two sets of numbers, say the first four multiples of 3 in set $A$:

$ A = \{3,6,9,12\}$

and the first four multiples of 2 in set $B$:

$ B = \{2,4,6,8\} $.

If you want to know how many elements are in set $A$ versus $B$, you can't simply sum up the elements, because the two sets have elements in common.

In combinational mathematics, the inclusion-exclusion principle is a counting technique that solves this problem.

When having two sets, the method for counting the number of elements in the union of two finite sets is given by:

$\mid A \cup B \mid = \mid A \mid + \mid B \mid - \mid A \cap B \mid $,

where the horizontal lines denote the *cardinality* of a set, which is the number of elements in the set, considering a set with a finite number of elements. 

The formula expresses the fact that the sum of the sizes of the two sets may be too large since some elements may be counted twice. For the double-counted elements, one is subtracted again.

This formula can be extended to three sets, four sets, etc. For example, imagine you have a third set $C$. The number of elements in the union of three finite sets is given by:


$\mid A  \cup B\cup C \mid = \mid A \mid + \mid B \mid + \mid C \mid - \mid A \cap B \mid -\mid A \cap C \mid - \mid B \cap C \mid + \mid A \cap B \cap C \mid $

<img src="images/new_venn_diagram.png" width="350"/>


## Summary

In this Appendix section, you learned a bit more about set notation, and the difference between subsets and proper subsets. After that, you learned about how to count the number of elements in the union of sets using the inclusion-exclusion principle. You'll have a chance to work through problems related to the inclusion-exclusion principle in a related lab in this Appendix.
