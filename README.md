Find Middle Letters
Simple Python utility to find the middle letter(s) of a word.
ВНЁС ИЗМЕНЕНИЯ
Overview
This script finds the middle character(s) in a given word:

For odd‑length words — returns the single middle letter.

For even‑length words — returns two middle letters.

How It Works
The algorithm:

Calculates the word length.

Checks if the length is even or odd.

For even length: returns characters at positions (n/2 − 1) and n/2.

For odd length: returns the character at position n//2.

Usage
Run the script.

Enter a word when prompted.

The program will output the middle letter(s).

Examples:

Input: hello → Output: l (odd length: 5, middle at index 2)

Input: test → Output: es (even length: 4, middle at indices 1–2)

Input: python → Output: th (even length: 6, middle at indices 2–3)

Input: a → Output: a (single character)

Code Example
python
def find_middle_letters(word):
    """
    Find the middle letter(s) of a word.
    
    Args:
        word (str): Input word
        
    Returns:
        str: Middle letter (for odd length) or two middle letters (for even length)
    """
    length = len(word)
    if length % 2 == 0:
        middle_index = length // 2
        return word[middle_index - 1:middle_index + 1]
    else:
        middle_index = length // 2
        return word[middle_index]

# Example usage
word = input("Введите слово и нажмите ввод: ")
result = find_middle_letters(word)
print(f"Вывод: {result}")
Installation and Running
Prerequisites
Python 3.6 or higher

Steps
Clone the repository:

bash
git clone <repository-url>
cd find-middle-letters
Run the script:

bash
python find_middle_letters.py
Enter a word and press Enter.

View the result in the console.

Input and Output
Input: Any string (word) entered via console input.
Output: String with one or two characters — the middle letter(s) of the input word.

Edge Cases Handled
Single character: Returns that character.

Empty string: Will return an empty string (no error).

Even‑length words: Returns two middle characters.

Odd‑length words: Returns the single middle character.

Contributing
Contributions are welcome! You can help improve this project by:

Reporting bugs via Issues.

Suggesting new features.

Submitting pull requests with improvements.

Guidelines for contributions:

Add docstrings for new functions.

Keep code readable and well‑commented.

Test your changes before submitting.

License
This project is licensed under the MIT License — see the  file for details.

Contact
For questions or suggestions, please:

Open an issue on GitHub.

Contact the maintainer via GitHub messages.

