# Character-in-a-string
text = input("Enter a string: ")
char_count = {}
for char in text:
    if char!= " ":
        if char in char_count:
            char_count[char] += 1
        else:
            char_count[char] = 1
most_frequent = max(char_count, key=char_count.get)
frequency = char_count[most_frequent]
print(f"The most frequent character is '{most_frequent}' which appears {frequency} times.)
