# Recursion
Checkpoint on Recursion

The If-else statement was used as seen in the code and the explanation is as follows:

BEGIN
    IF (start >= end) THEN
        RETURN true
This block checks if the current substring being considered is empty or has only one character (i.e., start is greater than or equal to end). 
If so, it means that the substring is either empty or has only one character, and in such cases, the function returns true, indicating that it is a palindrome.

   IF (word[start] === word[end]) THEN
        RETURN isPalindrome(word, start + 1, end - 1)
If the condition above is not met, the code checks if the characters at positions 'start and 'end' within the word are the same. 
If they are equal, it means the current substring is a palindrome. 
In this case, the function calls itself recursively with the updated indices start + 1 and end - 1 to check the next inner substring.

   ELSE
        RETURN false
If the characters at positions start and end are not equal, the function returns false, indicating that the input word is not a palindrome.
