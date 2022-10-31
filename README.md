# 20221031-PY
2022-10-31 
This problem was asked by Google.
You are given a set of synonyms, such as (big, large) and (eat, consume). Using this set, determine if two sentences with the same number of words are equivalent.

For example, the following two sentences are equivalent:

"He wants to eat food."
"He wants to consume food."
Note that the synonyms (a, b) and (a, c) do not necessarily imply (b, c): consider the case of (coach, bus) and (coach, teacher).

Follow-up: what if we can assume that (a, b) and (a, c) do in fact imply (b, c)?

Solution
For the first problem, we must create a data structure that allows us to simply check whether any two words are synonyms. We can achieve this by making a dictionary whose keys are all the distinct words in our set, and whose values are their synonyms.

Once we have this data structure, we will split each sentence into words and iterate over each pair. If for every pair, either the words are identical, or one word can be found as a value corresponding to the other's key, then the two sentences are equivalent.
