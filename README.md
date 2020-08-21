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

10. Все классы являются наследниками класса *object*.

11. Объекты внутреннего класса могут быть созданы только внутри внешнего класса. Внутренний класс имеет доступ ко всем полям внешнего класса. Ссылку на объект внешнего класса из внутреннего класса можно получить с помощью выражения *внешний_класс.this*. Внутренние классы можно объявить внутри любого контекста (метод, цикл, ...). Объект внешнего класса не может ссылаться на объект внутреннего класса.

12. Можно передать переменной суперкласса ссылку на объект производного класса, но она не сможет использовать его поля и методы (только через объект производного класса). Объект производного класса не может ссылаться на свой базовый.

13. **final** запрещает наследование класса, а также переопределение методов.

14. Несмотря на то, что переменная представляет объект базового класса, виртуальная машина видит, что в реальности она указывает на объект производного класса. Поэтому при вызове методов у этого объекта будет вызываться та версия метода, которая определена в базовом классе, а не в производном.
