# Задача A-5. Форматирование строк с тегом `div`
Реализуйте функцию
```objectivec
char** div_format(char **s) {
    // ...
}
```

и программу, использующую эту функцию для форматирования текстовой разметки состоящей из `<div>`, `</div>` и ASCII
строк.
Правильное форматирование подразумевает расстановку 4х пробелов согласно вложенности. То есть в исходном тексте
необходимо игнорировать все *ведущие* и *закрывающие* пробелы, и форматировать вывод строк простановкой нового
соответствующего количества пробелов. В случае некорректной последовательности тэгов, выведите в поток вывода `[error]`.

**ВАЖНО! Программа в любом случае должна возвращать `0`. Не пишите `return -1`, `exit(1)` и т.п. Даже если обнаружилась
какая-то ошибка, все равно необходимо вернуть `0`! (и напечатать `[error]` в *stdout*).**

## Examples
### Input
```xml
<div> cheburashka <div>
pozdno el kofe i </div> slivki </div>
```
### Output
```xml
<div>
    cheburashka
    <div>
        pozdno el kofe i
    </div>
    slivki
</div>
```