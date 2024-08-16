import requests

github_url = "https://raw.githubusercontent.com/Katherine-Brown-8000/Counting-letters-in-a-text/main/book_genres"

def download_file_from_github(url):
    response = requests.get(url)
    if response.status_code == 200:
        return response.text.strip()
    else:
        raise Exception(f"failed to download file: {response.status_code}")

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

text = download_file_from_github(github_url)

result = count_letters(text)
print(result)

# uncomment print to show text in file
# print(text)
