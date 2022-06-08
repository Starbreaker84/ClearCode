xchange - сhanged // логический флажок, указывающий была ли произведена хотя бы одна перестановка значений при сортировке (функция MadMax)

item - сurrentNumber // текущее значения из массива для перестановки элементов при сортировке (функция MadMax)

code - unlockCode // код разблокировки телефона (функция PatternUnlock)

line - lengthOfUnlockLine // длинна линии разблокировки телефона (функция PatternUnlock)

checker - sumOfBesideDigits // сумма стоящих рядом цифр для анализа является ли линия между ними диагональю (функция PatternUnlock)

result - sumOfAllOtherNumbers // число, равное сумме всех остальных чисел (функция SumOfThe)

sum - sumOfNumbers // число, равное сумме всех чисел (моя приватная функция в функции SumOfThe)

s - stringForEncode // строка для шифровки (моя приватная функция в функции TheRabbitsFoot)

s - stringForDecode // строка для дешифровки (моя приватная функция в функции TheRabbitsFoot)

sLen - stringForEncodeLength // длинна строки для шифровки (моя приватная функция в функции TheRabbitsFoot)

sLen - stringForDecodeLength // длинна строки для дешифровки (моя приватная функция в функции TheRabbitsFoot)

rows - numberOfRowsInMatrix // кол-во строк в матрице (моя приватная функция в функции TheRabbitsFoot)

cols - numberOfColumnsInMatrix // кол-во столбцов в матрице (моя приватная функция в функции TheRabbitsFoot)

chars - indexOfCharInString // индекс символа в строке для шифровки/дешифровки (моя приватная функция в функции TheRabbitsFoot)

words - wordsFromStringForDecode // массив отдельных слов из входящей строки (моя приватная функция в функции TheRabbitsFoot)

stringForEncode - encodedString // зашифрованная строка - тут надо пояснить, изначально я как раз некорректно использовал одну переменную и для ввода изначальной строки и для вывода результата, поэтому сделал маленький рефакторинг и добавил новую переменную, поэтому тут скорее не переименование а исправление ошибки в соответствии с п. 3 занятия (вообще я уже вижу что эта переменная в принципе не нужна, но пока оставлю для рефакторинга, может на следующих занятиях пригодится)

stringForDecode - decodedString // дешифрованная строка - пояснение аналогичное предыдущему

printCost - totalPrintingCost // итоговая стоимость печати (функция PrintingCosts)

values - characterPrintingCosts // массив стомостей печати каждого символа (функция PrintingCosts)

keys - characterTable // таблица симоволов (функция PrintingCosts)

index - indexOfCharacterTable //индекс символа в таблице символов (функция PrintingCosts)

*Ух... я что-то увлекся, кстати, заметил интересную штуку - программы, где поработал над именами и немного над рефакторингом, стали буквально "читаться", как книга.*
