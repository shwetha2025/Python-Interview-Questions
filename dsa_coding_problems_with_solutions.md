# 1. Longest Substring Without Repeating Characters
# Find the length of the longest substring without any repeated characters.
    substring = "abcabcbb"
    sub_set = set()
    li1 = []
    for each in substring:
        if each not in sub_set:
            sub_set.add(each)
        else:
            length = len(sub_set)
            li1.append(length)
            sub_set = set()
            sub_set.add(each)
    
    print(max(li1))
    print(li1)
