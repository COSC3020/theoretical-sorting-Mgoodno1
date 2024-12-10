# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.

Answer:
To verify the claim of an O(n) sorting algorithm based on comparisons, we would first test it empirically with sorted, reversed, and randomly shuffled data to see if the runtime remains linear and consistently fast, particularly on larger inputs. However, from a theoretical perspective, the claim contradicts the well-established result that comparison-based sorting algorithms have a lower bound of O(n log n), as proven by the decision tree model. This lower bound arises because sorting involves distinguishing among n! permutations, requiring at least O(n log n) comparisons. Therefore, such a sorting algorithm cannot exist, and the claim is likely incorrect.
