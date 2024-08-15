text = 'cats'

def count_letters(text):
    text = text.lower()

    letter_count = {}

    for char in text:
        if char.isalpha():
            if char in letter_count:
                letter_count[char] += 1
            else:
                letter_count[char] = 1

    return letter_count

result = count_letters(text)
print(result)
