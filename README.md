# Laba_6
Лабораторная работа №6
def find_middle_letters(word):
    # вычисляем длину слова
    length = len(word)
    # если длина чётная
    if length % 2 == 0:
    # находим две средние буквы
        middle_index = length // 2
        return word[middle_index - 1:middle_index + 1]
    else:
     # если длина нечётная
     # находим одну среднюю букву
        middle_index = length // 2
        return word[middle_index]
# Пример
word = input("Введите слово и нажмите ввод: ")
result = find_middle_letters(word)
#вывод, ответ
print(f"Вывод: {result}")
