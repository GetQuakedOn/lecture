# Java

1. *String* - неизменяемый класс, и когда происходит конкатенация строк, то создается новая строка со старым текстом и новым. Название переменной будет ссылаться на новый объект.

2. Ссылочная переменная с модификатором **final** будет привязана к определенному объекту без возможности её как-либо отвязать (переопределить или приравнять к null). **final** действует только на ссылку, а на сам объект влияния не оказывает. 

3. *Scanner* закрываем обязательно.

4. Каждый объект имеет 3 измерения: идентификатор, атрибуты и поведение.

5. Статические поля и методы являются полями и методами класса, а не объекта.

6. К **super** конструктору можно и нужно обратиться только в конструкторе наследника, первой строчкой.

7. **super** должно идти первой строчкой.

8. **protected** делает поля видимыми только для подклассов.

9. В Java невозможно создать объект в стеке.

10. Все классы являются наследниками класса *Object*.

11. Объекты внутреннего класса могут быть созданы только внутри внешнего класса. Внутренний класс имеет доступ ко всем полям внешнего класса. Ссылку на объект внешнего класса из внутреннего класса можно получить с помощью выражения *внешний_класс.this*. Внутренние классы можно объявить внутри любого контекста (метод, цикл, ...). Объект внешнего класса не может ссылаться на объект внутреннего класса.

12. Можно передать переменной суперкласса ссылку на объект производного класса, но она не сможет использовать его поля и методы (только через объект производного класса). Объект производного класса не может ссылаться на свой базовый.

13. **final** запрещает наследование класса, а также переопределение методов.

14. Несмотря на то, что переменная представляет объект базового класса, виртуальная машина видит, что в реальности она указывает на объект производного класса. Поэтому при вызове методов у этого объекта будет вызываться та версия метода, которая определена в базовом классе, а не в производном.

15. Производный класс обязан переопределить и реализовать все абстрактные методы, которые имеются в базовом абстрактном классе.

16. Правила Переопределения Методов:
      - Должны иметь одинаковые возвращаемый тип и аргументы 
      - Уровень доступа может быть более ограничивающим, чем уровень доступа переопределенных методов. (Например: Если метод суперкласса объявлен как **public**, то переопределенный метод в подклассе не может быть ни **private** ни **protected**)
      - Метод, объявленный с помощью ключевых слов **final** или **static** не может быть переопределен 
      - Если метод не может быть наследован, то он не может быть переопределен 
      - Конструкторы не могут быть переопределены

17. **interface** может содержать только **static final** переменные.
      - Не могут содержать конструктор, потому что интерфейсы не могут инстанцироваться.
      - Интерфейсы могут расширять другие интерфейсы.
      - Класс может реализовать любое количество интерфейсов.

18. Класс может наследоваться лишь от одного суперкласса, но может реализовывать множество интерфейсов.

19. При сравнении объектов сравниваются ссылки, а не значения

20. (*object* **instanceof** *class*) -  проверяет, создан ли объект на основе класса.

21. Если нам надо применить в классе несколько интерфейсов, то они все перечисляются через запятую после **implements**.

22. В интерфейсы включены:
      - Методы по умолчанию
      - Статические методы
      - Приватные методы
      - Статические константы
      - Множественная реализация интерфейсов
      - Наследование интерфейсов
      - Вложенные интерфейсы
      
23. *Метод по умолчанию* в интерфейсе помечается оператором **default**

24. При восходящем преобразовании *(baseclass = subclass; baseclass **.** ... )* вызываются те методы, которые принадлежат базовому классу, но выводятся производные классы. (Интерфейс получает базового класса, но вывод ссылается на производный класс).

25. При создании обобщенного метода универсальный параметр указывается перед типом возвращаемого значения.

26. При наследовании от обобщенного класса класс-наследник должен передавать данные о типе в конструкторе базового класса.

27. Объект одного обобщенного типа можно привести к другому типу, если они используют один и тот же тип.

28. Метод *toString()* вызывается неявно когда выводится объект класса и **this**.

29. Для сырого типа по-умолчанию типом параметризации является **Object**.

30. В **Set**.*contains(**Object** o)* используется хеширование.

31. Если *hashCode()* одинаковый, то вызывается *equals()*.

32. Реализуем **Runnable** и передаем объект в конструктор **Thread**. 

33. **volatile** не кэшируется.

34. **synchronized** применяется только к методам и блокам кода.

нахуй пиздуйте с моей странички 
