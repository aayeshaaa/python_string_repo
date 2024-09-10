# python_string_repo
leetcod python string portion
<br>
Valid Palindrome
<br>

class Solution(object):
    def check_palindrome(self,s):
# remove_alphanumerics
        s =  ''.join(char for char in s if char.isalnum())
# all upper case to lower 
        s =  s.lower()

# reverse of the string 
        reversed_string = ''.join(reversed(s)) 
        # return reversed_string
# check if the string and its reverse are equal 
        if s == reversed_string:
            return True
        else:
            return False
obj = Solution()

result = obj.check_palindrome('A man, a plan, a canal: Panama')
print(result)

