# У имени переменной отсутствует префикс расширения

Все добавленные объекты (методы и объекты, отчеты, обработки и подсистемы, а также обработчики событий) расширения, 
а также имена собственных методов и переменных расширяющих модулей, должны иметь префикс, 
соответствующий префиксу самого расширения.

## Неправильно

```bsl
&Before("NonComplient")
Процедура Ext1_НеправильныйМетод()
    Ext_Переменная = Истина;
КонецПроцедуры
```

## Правильно

```bsl
&After("Complient")
Процедура Ext1_ПравильныйМетод()
    Ext1_Переменная = Истина;
КонецПроцедуры
```

## См.


- [Требования к программным продуктам](https://1c.ru/rus/products/1c/predpr/compat/soft/requirements.htm)