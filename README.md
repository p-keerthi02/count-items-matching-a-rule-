class Solution:
    def countMatches(self, items: List[List[str]], rulekey: str, rulevalue: str) -> int:
        if rulekey == "type":
            index = 0
        elif rulekey == "color":
            index = 1
        elif rulekey == "name":
            index = 2
        x = 0
        for i in items:
            if i[index] == rulevalue:
                x += 1
        return x 
