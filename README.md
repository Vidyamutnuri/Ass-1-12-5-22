# Ass-1-12-5-22
Assignment-1
class Solution:
    def isValid(self, s: str) -> bool:
        pair = dict(('()', '[]', '{}'))
        stk= []
        for x in s:
            if x in '([{:
            stk.append(x)
            elif len(stk) == 0 or x != pair[stk.pop()]:
                return False
        return len(stk) == 0
                
