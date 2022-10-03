# tests_for_java

ТЕСТИРОВАНИЕ ЗНАНИЙ ПО JAVA
В этом тесте приведено некоторое кол-во алгоритмических задач начального уровня и теоретических вопросов по основам Java.

Ваша цель при решении задач – достичь, по крайней мере, 70% по производительности. Время решения каждого упражнения - не более 20-30 минут.
Задачи выбраны на Leetcode - вам нужно будет зарегистрироваться.

В разделе теории некоторые вопросы - на английском.

Если вы уверенно решили все задачи, уложились во время и нужную производительность, а также свободно отвечаете на приведенные теоретические вопросы, то вы - молодец, у вас хорошая база и начинающая группа не для вас.

Если же вы поняли, что вам не хватает знаний, тогда я вас обрадую - вы их можете получить! Подробнее ознакомиться с занятиями в моей онлайн-группе вы можете здесь ➡ На главную

АЛГОРИТМИЧЕСКАЯ ЧАСТЬ
Массивы:

Contains Duplicate
Occurrences After Bigram
Find Words That Can Be Formed by Characters
Can Make Arithmetic Progression From Sequence
Average Salary Excluding the Minimum and Maximum Salary
Sort Array By Parity II
Relative Sort Array
Reorder Data in Log Files
Shuffle String
Check Array Formation Through Concatenation
Matrix Cells in Distance Order
Maximum Units on a Truck
Строки:

Defanging an IP Address
Find First Palindromic String in the Array
Check if the Sentence Is Pangram
Goal Parser Interpretation
First Unique Character in a String
Keyboard Row
Positions of Large Groups
Uncommon Words from Two Sentences
ArrayList:

Kids With the Greatest Number of Candies
Summary Ranges
Find Common Characters
Arithmetic Subarrays
Check Array Formation Through Concatenation
Minimum Subsequence in Non-Increasing Order
String Matching in an Array
LinkedList:

Palindrome Linked List
Remove Linked List Elements
Intersection of Two Linked Lists
Convert Binary Number in a Linked List to Integer
Map:

Number of Good Pairs
Two Sum
Number of Good Pairs
Maximum Number of Balloons
Find the Town Judge
Verifying an Alien Dictionary
Set:

Fair Candy Swap
Contains Duplicate
Intersection of Two Arrays
N-Repeated Element in Size 2N Array
Check If N and Its Double Exist
Design HashSet
Destination City
Path Crossing
ТЕОРЕТИЧЕСКИЕ ВОПРОСЫ
Basic:

Какие примитивные типы данных в Java вы знаете?
Расскажите о классах-обертках (wrapper classes)? Зачем они нужны?
Что такое автоупаковка (autoboxing)?
Все ли строки в Java являются неизменяемыми (immutable)?
Где хранятся строки в Java?
Что такое класс?
Что вы знаете о методе equals()? Какие правила нужно учитывать, переопределяя метод equals()?
Какие виды наследования в Java вы знаете?
Что такое перегрузка методов (overloading)?
Скомпилируется ли данный пример?
public class Man extends Human {
    String name;
    public Man() {
        this.name = "Anna";
        super();
    }
}
Что НЕ наследуется подклассом от суперкласса?
Скомпилируется ли данный код?
class A {
    int x;
    public A(int x) {
        this.x = x;
    }
}

class B extends A {
    String s;
    public B(String s) {
        this.s = s;
    }
}
Как убрать возможность наследования класса?
Exceptions:

Когда возникает необходимость в блоке finally?
При каких сценариях блок finally НЕ будет исполнен?
Возможно ли использовать блок try без блока catch?
Каков будет результат после выполнения данных методов?
public static void add() {
    Amount amount = new Amount(Currency.EURO, 2);
    Amount amount2 = new Amount(Currency.RUB, 2);
    try {
        amount.add(amount2); //выбрасывает CurrenciesDoNotMatchException
    } catch (Exception e){
        System.out.println("Some exception occurs: " + e);
    } catch (CurrenciesDoNotMatchException e) {
        System.out.println("Currencies do not match: " + e);
    }
}
Объясните применение концепции try-with-resources
Расскажите о best practices обработки исключений
Наследование:

Are constructors and initializers also inherited to sub classes in Java?
Are static members inherited to sub classes in Java?
Can we change argument list of overridden method?
Can we override a method which throws run-time exception without throws clause?
Can we override final method in Java?
What is the difference between Polymorphism and Inheritance?
Difference between method overloading and overriding?
What will be the output of following program?
class A {
    int i = 10;
}

class B extends A {
    int i = 20;
}

public class MainClass {
    public static void main(String[] args) {
        A a = new B();
        System.out.println(a.i);
    }
}
Проанализируйте код, предугадайте значение переменной actual и впишите правильное значение в переменную result, чтобы получить Test passed.
public static void main(String[] args) {
    Sub sub = new Sub();
    sub.method();

    String result = "?"; // впишите правильное значение
    String actual = sub.x + "" + sub.y;
    if (result.equals(actual)) {
        System.out.println("Test passed");
    } else {
        System.out.println("Test fails");
    }
}

static class Super {
    static int x;
    int y;

    public Super() {
        this(10);
    }

    public Super(int y) {
        this.y = y;
        x += 2;
    }
}

static class Sub extends Super {
    public Sub() {
        x += 5;
        y += 2;
    }

    public Sub(int z) {
        x += 5;
        y += z;
    }

    public Sub method() {
        return new Sub(5);
    }
}
Интерфейсы:

Что такое интерфейс?
Если в интерфейсе указано поле, то какими характеристиками оно обладает по умолчанию?
Какими свойствами НЕ могут обладать члены в интерфейсах?
Какие модификаторы НЕ могут иметь методы в интерфейсах?
Какая разница между следующими обозначениями методов в интерфейсах?
void methodOne();
public void methodOne();
abstract void methodOne();
public abstract void methodOne();
Для чего используются default-методы в интерфейсе?
Можно ли создать объект интерфейса?
Корректен ли данный код? Если нет, то в чем ошибка? Как исправить код?
interface Test {
    int x;
    void foo();
}   
Что такое функциональный интерфейс? Приведите примеры.
Что такое маркер-интерфейс (marker / tag interface)?
Можно ли применять extends в интерфейсах? Корректен ли данный код?
interface Currency {
    double getCurrency();
}
interface Time {
    double getTime();
}
interface TimeCurrency extends Time, Currency {
}   
Почему интерфейсы не имеют конструктора, а абстрактные классы имеют?
Чем отличается интерфейс от абстрактного класса?
Can we create non static variables in an interface?
What will happen if we do not initialize variables in Java interface?
When we need to use extends and implements?
Can we declare interface as final?
Can we declare constructor inside an interface?
How can we access same variables defined in two interfaces implemented by a class?
Can we re-assign a value to a field of interfaces?
Can we override an interface method with visibility other than public?
Can interfaces have static methods?
What is the use of extending an interface?
Advantage and disadvantages of Interfaces
Абстрактные классы:

Что такое абстрактный класс?
Как определяются и что такое абстрактные методы?
Abstract class must have only abstract methods. True or false?
Why final and abstract can not be used at a time?
Can we declare abstract methods as private? Justify your answer?
Can we declare abstract methods as static?
We can’t instantiate an abstract class. Then why constructors are allowed in abstract class?
Can we declare abstract methods as synchronized?
Can we declare local inner class as abstract?
Is it possible to create abstract and final class in Java?
Is it possible to have an abstract method in a final class?
Вложенные классы:

Что такое вложенный класс (Nested class)?
Какие модификаторы доступа могут быть у вложенных классов (nested classes)?
Что вы можете рассказать о статическом вложенном классе?
Можно ли создать несколько экземпляров статического вложенного класса?
Чем отличаются статические вложенные классы от обычных внутренних классов?
Какие члены могут иметь вложенные классы?
Что такое анонимный класс?
Для чего можно использовать анонимный класс?
Что вы знаете о локальных внутренних классах?
Какой будет результат выполнения данного кода?
public class Outer {
    private int getValue(int data) {
        static class Inner {
            private int getData() {
                System.out.println("Inside inner class");
                if(data < 10) {
                    return 5;
                }
                else {
                    return 15;
                }
            }
        }
        Inner inner = new Inner();
        return inner.getData();
    }
    public static void main(String[] args) {
        Outer outer = new Outer();
        System.out.println(outer.getValue(10));
    }
}
Полиморфизм:

Что такое полиморфизм?
Какие виды полиморфизма вы знаете?
Что вы можете сказать о Runtime polymorphism? Приведите примеры?
Опишите проблемы полиморфизма
Что такое перегрузка оператора?
Какой результат выполнения метода main()?
class Base {
    public void fun() { 
        System.out.println("Base fun");      
    } 
} 
    
class Derived extends Base { 
    public void fun() {
        System.out.println("Derived fun");   
    } 
    public static void main(String[] args) { 
        Base obj = new Derived(); 
        obj.fun(); 
    }   
}
Проанализируйте код, предугадайте значение переменной actual и впишите правильное значение в переменную result, чтобы получить Test passed.
public static void main(String[] args) {
    A a = new B();
    B b = new B();
    add(a);
    add(b);

    String result = "?"; // впишите правильное значение
    String actual = a.x + " " + b.x;
    if (result.equals(actual)) {
        System.out.println("Test passed");
    } else {
        System.out.println("Test fails");
    }
}

public static void add(A a){
    a.x += 20;
}

static class A {
    int x = 5;
}

static class B extends A {
    int x = 10;
}
ArrayList:

Difference between List and ArrayList?
How do you increase the current capacity of an ArrayList?
How do you convert an ArrayList to Array?
Difference between length() of array and size() of ArrayList in Java?
Can we add more elements to an array list that has been marked as final?
What is the difference between ArrayList and LinkedList?
How to replace all occurrences of specified element of ArrayList?
How to prevent the addition of duplicate elements to ArrayList? What is the time and space complexity of suggested approaches?
When to use Array of ArrayList?
How to synchronize ArrayList in Java?
Difference between ArrayList and HashMap in Java?
What is the quickest way to find count of duplicate elements in an ArrayList, without using iteration or loops?
How can we create an ArrayList of unique values?
Describe fail-fast and fail-safe iterators
Linked List:

Какие типы связных списков вы знаете?
Расскажите как вставить данные в начало односвязного списка (Singly Linked List)?
Какое наибольшее преимущество связного списка?
Как удалить первый узел из связного однонаправленного списка?
Set:

Какими свойствами обладает Set?
Какими свойствами обладает HashSet?
Какая иерархия Set?
Какие правила для переопределения hashCode()?
Как конвертировать Set в List?
What interfaces are implemented by the HashSet class? What is the superclass of HashSet class?
How HashSet works internally in Java?
What is the default initial capacity and initial load factor of HashSet object?
Why does HashSet implementation in Java use HashMap as its backing?
What is TreeSet?
How TreeSet internally works in Java?
What is the difference between HashSet and TreeSet?
How to find elements of a TreeSet which are greater than or equal to the specified element?
Какой результат кода?
TreeSet<String> tree = new TreeSet<>((s1, s2) -> s2.length() -
s1.length());
tree.addAll(Arrays.asList("B", "C", "D", «A"));
System.out.println("Size: " + tree.size());
Расскажите о LinkedHashSet
Какие интерфейсы реализует LinkedHashSet?
Как удалить дубликаты из строки, сохранив порядок букв?
Пример: «abcabcdedd» => «abcde»
What is the difference between Set and Map?
Map:

Что такое хэширование?
Describe Java Map Hierarchy
Какие реализации интерфейса Map вы знаете?
What are the features of HashMap?
Что такое load factor?
What is rehashing?
How is HashMap Implemented in Java? How does its implementation use hashcode() and equals() methods of objects?
What collection views of a map interface?
Что вы знаете о методе hashCode()?
Implement a method of merging two maps
Условие: даны 2 maps - <id, message>. Нужно объединить эти maps так, чтобы при
одинаковых id текст сообщения message конкатенировался.
Сделать в 2 строки кода.
public Map<Integer, String> merge(Map<Integer, String> map1, Map<Integer, String> map2) {
    // your code
}
Расскажите о LinkedHashMap
Расскажите о TreeMap
What is an internal implementation of TreeMap?
Может ли TreeMap содержать ключ равный null?
Как конвертировать TreeMap в ArrayList?
Как получить первый и последний элемент в TreeMap?
