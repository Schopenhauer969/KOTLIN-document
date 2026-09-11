# Kotlin — Beginner to Advanced

> A complete Kotlin learning guide from **Beginner → Intermediate → Advanced**, with English + Khmer explanations and practical code examples.

---

## 📚 Table of Contents

* [1. What is Kotlin?](#1-what-is-kotlin)
* [2. Installation](#2-installation)
* [3. Your First Kotlin Program](#3-your-first-kotlin-program)
* [4. Comments](#4-comments)
* [5. Variables](#5-variables)
* [6. Data Types](#6-data-types)
* [7. Type Conversion](#7-type-conversion)
* [8. Strings](#8-strings)
* [9. Operators](#9-operators)
* [10. Input and Output](#10-input-and-output)
* [11. If / Else](#11-if--else)
* [12. When](#12-when)
* [13. Loops](#13-loops)
* [14. Ranges](#14-ranges)
* [15. Functions](#15-functions)
* [16. Default and Named Arguments](#16-default-and-named-arguments)
* [17. Single Expression Functions](#17-single-expression-functions)
* [18. Null Safety](#18-null-safety)
* [19. Arrays](#19-arrays)
* [20. Lists](#20-lists)
* [21. Sets](#21-sets)
* [22. Maps](#22-maps)
* [23. Collections Operations](#23-collections-operations)
* [24. Classes](#24-classes)
* [25. Constructors](#25-constructors)
* [26. Properties](#26-properties)
* [27. Inheritance](#27-inheritance)
* [28. Abstract Classes](#28-abstract-classes)
* [29. Interfaces](#29-interfaces)
* [30. Data Classes](#30-data-classes)
* [31. Enum Classes](#31-enum-classes)
* [32. Sealed Classes](#32-sealed-classes)
* [33. Objects and Singleton](#33-objects-and-singleton)
* [34. Companion Objects](#34-companion-objects)
* [35. Extension Functions](#35-extension-functions)
* [36. Scope Functions](#36-scope-functions)
* [37. Lambdas](#37-lambdas)
* [38. Higher-Order Functions](#38-higher-order-functions)
* [39. Generics](#39-generics)
* [40. Variance](#40-variance)
* [41. Exception Handling](#41-exception-handling)
* [42. Custom Exceptions](#42-custom-exceptions)
* [43. File Handling](#43-file-handling)
* [44. Equality](#44-equality)
* [45. Destructuring](#45-destructuring)
* [46. Operator Overloading](#46-operator-overloading)
* [47. Delegation](#47-delegation)
* [48. Lazy Initialization](#48-lazy-initialization)
* [49. lateinit](#49-lateinit)
* [50. Inline Functions](#50-inline-functions)
* [51. Reified Types](#51-reified-types)
* [52. Coroutines](#52-coroutines)
* [53. Suspend Functions](#53-suspend-functions)
* [54. Coroutine Dispatchers](#54-coroutine-dispatchers)
* [55. Structured Concurrency](#55-structured-concurrency)
* [56. Flow](#56-flow)
* [57. Channels](#57-channels)
* [58. Generics + Constraints](#58-generics--constraints)
* [59. DSL Concepts](#59-dsl-concepts)
* [60. Advanced Kotlin Project Structure](#60-advanced-kotlin-project-structure)
* [61. Best Practices](#61-best-practices)
* [62. Learning Roadmap](#62-learning-roadmap)

---

# 1. What is Kotlin?

## English

Kotlin is a modern, statically typed programming language developed by JetBrains.

Kotlin can be used for:

* Android development
* Backend development
* Server applications
* Desktop applications
* Multiplatform applications
* Web development
* Command-line applications

Kotlin is designed to work very well with Java.

## Khmer

Kotlin គឺជា programming language ទំនើបមួយ ដែលបង្កើតដោយ JetBrains។

Kotlin អាចប្រើសម្រាប់៖

* Android
* Backend
* Server
* Desktop
* Multiplatform
* Web
* Command-line applications

Kotlin អាចធ្វើការជាមួយ Java បានយ៉ាងល្អ។

---

# 2. Installation

You can use:

* IntelliJ IDEA
* Android Studio
* Kotlin compiler
* Gradle

For beginners, **IntelliJ IDEA** is a good choice for learning Kotlin.

---

# 3. Your First Kotlin Program

```kotlin
fun main() {
    println("Hello, Kotlin!")
}
```

Output:

```text
Hello, Kotlin!
```

### Explanation

`fun` means function.

`main()` is the entry point of the application.

`println()` prints text to the console.

### Khmer

`fun` មានន័យថា function។

`main()` គឺជាចំណុចចាប់ផ្តើមរបស់ program។

`println()` ប្រើសម្រាប់បង្ហាញអត្ថបទទៅ console។

---

# 4. Comments

## Single-line comment

```kotlin
// This is a comment
println("Hello")
```

## Multi-line comment

```kotlin
/*
    This is a
    multi-line comment
*/
println("Hello")
```

Comments are ignored by the compiler.

### Khmer

Comment គឺជាអត្ថបទសម្រាប់ពន្យល់ code ហើយ compiler មិន execute វាទេ។

---

# 5. Variables

Kotlin has two main variable declarations:

* `val`
* `var`

## val

`val` cannot be reassigned.

```kotlin
fun main() {
    val name = "Heng"

    println(name)
}
```

You cannot do:

```kotlin
val name = "Heng"
name = "Dara" // Error
```

## var

`var` can be changed.

```kotlin
fun main() {
    var age = 20

    age = 21

    println(age)
}
```

### English

Use `val` by default.

Use `var` only when the value needs to change.

### Khmer

គួរប្រើ `val` ជា default ព្រោះវាមិនអាចប្តូរតម្លៃបាន។

ប្រើ `var` នៅពេលតម្លៃត្រូវការប្តូរ។

---

# 6. Data Types

Common Kotlin types:

```kotlin
fun main() {
    val name: String = "Heng"
    val age: Int = 25
    val price: Double = 19.99
    val score: Float = 95.5f
    val isActive: Boolean = true
    val grade: Char = 'A'

    println(name)
    println(age)
    println(price)
    println(score)
    println(isActive)
    println(grade)
}
```

## Common Types

| Type    | Example   |
| ------- | --------- |
| String  | `"Hello"` |
| Int     | `100`     |
| Long    | `100000L` |
| Double  | `10.5`    |
| Float   | `10.5f`   |
| Boolean | `true`    |
| Char    | `'A'`     |
| Short   | `10`      |
| Byte    | `1`       |

### Khmer

Kotlin មាន data types ជាច្រើនសម្រាប់រក្សាទុកទិន្នន័យប្រភេទផ្សេងៗគ្នា។

---

# 7. Type Conversion

Kotlin does not automatically convert numeric types.

```kotlin
fun main() {
    val number: Int = 100

    val longNumber: Long = number.toLong()
    val doubleNumber: Double = number.toDouble()

    println(longNumber)
    println(doubleNumber)
}
```

Common conversions:

```kotlin
toInt()
toLong()
toDouble()
toFloat()
toShort()
toByte()
toString()
```

Example:

```kotlin
fun main() {
    val text = "123"

    val number = text.toInt()

    println(number + 10)
}
```

Output:

```text
133
```

---

# 8. Strings

```kotlin
fun main() {
    val name = "Heng"
    val age = 25

    println("Name: $name")
    println("Age: $age")
}
```

This is called **string interpolation**.

## Expressions inside strings

```kotlin
fun main() {
    val a = 10
    val b = 20

    println("Sum = ${a + b}")
}
```

Output:

```text
Sum = 30
```

## Multi-line strings

```kotlin
fun main() {
    val message = """
        Hello
        Kotlin
        Developer
    """.trimIndent()

    println(message)
}
```

---

# 9. Operators

## Arithmetic

```kotlin
fun main() {
    val a = 20
    val b = 6

    println(a + b)
    println(a - b)
    println(a * b)
    println(a / b)
    println(a % b)
}
```

## Comparison

```kotlin
fun main() {
    val a = 10
    val b = 20

    println(a == b)
    println(a != b)
    println(a > b)
    println(a < b)
    println(a >= b)
    println(a <= b)
}
```

## Logical operators

```kotlin
fun main() {
    val age = 25
    val hasTicket = true

    println(age >= 18 && hasTicket)
    println(age >= 18 || hasTicket)
    println(!hasTicket)
}
```

---

# 10. Input and Output

```kotlin
fun main() {
    print("Enter your name: ")

    val name = readln()

    println("Hello, $name")
}
```

Input:

```text
Heng
```

Output:

```text
Hello, Heng
```

## Reading numbers

```kotlin
fun main() {
    print("Enter your age: ")

    val age = readln().toInt()

    println("You are $age years old.")
}
```

---

# 11. If / Else

```kotlin
fun main() {
    val age = 20

    if (age >= 18) {
        println("Adult")
    } else {
        println("Minor")
    }
}
```

## Multiple conditions

```kotlin
fun main() {
    val score = 85

    if (score >= 90) {
        println("A")
    } else if (score >= 80) {
        println("B")
    } else if (score >= 70) {
        println("C")
    } else {
        println("F")
    }
}
```

## If as an expression

Kotlin's `if` can return a value.

```kotlin
fun main() {
    val age = 20

    val result = if (age >= 18) {
        "Adult"
    } else {
        "Minor"
    }

    println(result)
}
```

---

# 12. When

`when` is Kotlin's powerful conditional expression.

```kotlin
fun main() {
    val day = 3

    when (day) {
        1 -> println("Monday")
        2 -> println("Tuesday")
        3 -> println("Wednesday")
        4 -> println("Thursday")
        5 -> println("Friday")
        6 -> println("Saturday")
        7 -> println("Sunday")
        else -> println("Invalid day")
    }
}
```

## when as an expression

```kotlin
fun main() {
    val score = 85

    val grade = when {
        score >= 90 -> "A"
        score >= 80 -> "B"
        score >= 70 -> "C"
        score >= 60 -> "D"
        else -> "F"
    }

    println(grade)
}
```

### Khmer

`when` មានប្រយោជន៍ខ្លាំងសម្រាប់ condition ច្រើន ហើយអាចប្រើជំនួស `if / else if` ក្នុងករណីជាច្រើន។

---

# 13. Loops

## for loop

```kotlin
fun main() {
    for (i in 1..5) {
        println(i)
    }
}
```

Output:

```text
1
2
3
4
5
```

## while

```kotlin
fun main() {
    var i = 1

    while (i <= 5) {
        println(i)
        i++
    }
}
```

## do while

```kotlin
fun main() {
    var i = 1

    do {
        println(i)
        i++
    } while (i <= 5)
}
```

---

# 14. Ranges

```kotlin
fun main() {
    for (i in 1..5) {
        println(i)
    }
}
```

## Until

```kotlin
fun main() {
    for (i in 1 until 5) {
        println(i)
    }
}
```

Output:

```text
1
2
3
4
```

## DownTo

```kotlin
fun main() {
    for (i in 5 downTo 1) {
        println(i)
    }
}
```

## Step

```kotlin
fun main() {
    for (i in 1..10 step 2) {
        println(i)
    }
}
```

---

# 15. Functions

Basic function:

```kotlin
fun greet() {
    println("Hello Kotlin")
}

fun main() {
    greet()
}
```

## Parameters

```kotlin
fun greet(name: String) {
    println("Hello, $name")
}

fun main() {
    greet("Heng")
}
```

## Return value

```kotlin
fun add(a: Int, b: Int): Int {
    return a + b
}

fun main() {
    val result = add(10, 20)

    println(result)
}
```

---

# 16. Default and Named Arguments

## Default arguments

```kotlin
fun greet(name: String = "Guest") {
    println("Hello, $name")
}

fun main() {
    greet()
    greet("Heng")
}
```

## Named arguments

```kotlin
fun createUser(name: String, age: Int) {
    println("Name: $name")
    println("Age: $age")
}

fun main() {
    createUser(
        age = 25,
        name = "Heng"
    )
}
```

### Khmer

Named arguments ធ្វើឱ្យ code អានងាយ និងមិនងាយច្រឡំ parameter។

---

# 17. Single Expression Functions

Instead of:

```kotlin
fun add(a: Int, b: Int): Int {
    return a + b
}
```

You can write:

```kotlin
fun add(a: Int, b: Int): Int = a + b
```

Type inference can also be used:

```kotlin
fun add(a: Int, b: Int) = a + b
```

---

# 18. Null Safety

Null safety is one of Kotlin's most important features.

Without null safety:

```text
NullPointerException
```

can cause runtime problems.

## Nullable variable

```kotlin
fun main() {
    var name: String? = "Heng"

    name = null

    println(name)
}
```

The `?` means the variable can contain `null`.

---

## Safe call

```kotlin
fun main() {
    val name: String? = null

    println(name?.length)
}
```

Output:

```text
null
```

---

## Elvis operator

```kotlin
fun main() {
    val name: String? = null

    val result = name ?: "Unknown"

    println(result)
}
```

Output:

```text
Unknown
```

---

## let

```kotlin
fun main() {
    val name: String? = "Heng"

    name?.let {
        println("Name: $it")
    }
}
```

---

## Avoid unnecessary !!

The `!!` operator forces Kotlin to treat a nullable value as non-null.

```kotlin
val name: String? = "Heng"

println(name!!.length)
```

If `name` is null, this can throw an exception.

Prefer:

```kotlin
println(name?.length)
```

---

# 19. Arrays

```kotlin
fun main() {
    val numbers = arrayOf(10, 20, 30, 40)

    println(numbers[0])
    println(numbers[1])
}
```

Loop:

```kotlin
fun main() {
    val numbers = arrayOf(10, 20, 30)

    for (number in numbers) {
        println(number)
    }
}
```

---

# 20. Lists

## Immutable list

```kotlin
fun main() {
    val names = listOf(
        "Heng",
        "Dara",
        "Sok"
    )

    println(names)
}
```

## Mutable list

```kotlin
fun main() {
    val names = mutableListOf(
        "Heng",
        "Dara"
    )

    names.add("Sok")
    names.remove("Dara")

    println(names)
}
```

### Best practice

Prefer immutable collections when possible.

```kotlin
val names = listOf("Heng", "Dara")
```

---

# 21. Sets

A `Set` does not contain duplicate elements.

```kotlin
fun main() {
    val numbers = setOf(
        1,
        2,
        2,
        3,
        3
    )

    println(numbers)
}
```

Output:

```text
[1, 2, 3]
```

Mutable set:

```kotlin
fun main() {
    val numbers = mutableSetOf(1, 2, 3)

    numbers.add(4)
    numbers.remove(2)

    println(numbers)
}
```

---

# 22. Maps

Maps store key-value pairs.

```kotlin
fun main() {
    val users = mapOf(
        "admin" to "Admin User",
        "user1" to "Heng"
    )

    println(users["admin"])
}
```

Mutable map:

```kotlin
fun main() {
    val users = mutableMapOf(
        "admin" to "Admin User"
    )

    users["user1"] = "Heng"

    println(users)
}
```

---

# 23. Collections Operations

Kotlin provides powerful collection functions.

## map

```kotlin
fun main() {
    val numbers = listOf(1, 2, 3, 4)

    val doubled = numbers.map {
        it * 2
    }

    println(doubled)
}
```

Result:

```text
[2, 4, 6, 8]
```

## filter

```kotlin
fun main() {
    val numbers = listOf(1, 2, 3, 4, 5)

    val evenNumbers = numbers.filter {
        it % 2 == 0
    }

    println(evenNumbers)
}
```

## reduce

```kotlin
fun main() {
    val numbers = listOf(1, 2, 3, 4)

    val total = numbers.reduce { a, b ->
        a + b
    }

    println(total)
}
```

## forEach

```kotlin
fun main() {
    val names = listOf("Heng", "Dara", "Sok")

    names.forEach {
        println(it)
    }
}
```

---

# 24. Classes

A class defines the structure and behavior of an object.

```kotlin
class Person(
    val name: String,
    val age: Int
) {
    fun introduce() {
        println("My name is $name and I am $age years old.")
    }
}

fun main() {
    val person = Person("Heng", 25)

    person.introduce()
}
```

### Khmer

Class គឺជា blueprint សម្រាប់បង្កើត object។

Object គឺជា instance របស់ class។

---

# 25. Constructors

Primary constructor:

```kotlin
class User(
    val name: String,
    val age: Int
)

fun main() {
    val user = User("Heng", 25)

    println(user.name)
    println(user.age)
}
```

Secondary constructor:

```kotlin
class User(
    val name: String
) {
    var age: Int = 0

    constructor(name: String, age: Int) : this(name) {
        this.age = age
    }
}

fun main() {
    val user = User("Heng", 25)

    println(user.name)
    println(user.age)
}
```

---

# 26. Properties

```kotlin
class Person(
    var name: String,
    var age: Int
)

fun main() {
    val person = Person("Heng", 25)

    person.name = "Dara"
    person.age = 30

    println(person.name)
    println(person.age)
}
```

## Custom getter

```kotlin
class Rectangle(
    val width: Double,
    val height: Double
) {
    val area: Double
        get() = width * height
}

fun main() {
    val rectangle = Rectangle(10.0, 5.0)

    println(rectangle.area)
}
```

---

# 27. Inheritance

Classes are final by default.

Use `open` when a class should be inherited.

```kotlin
open class Animal {
    fun eat() {
        println("Animal is eating")
    }
}

class Dog : Animal() {
    fun bark() {
        println("Dog is barking")
    }
}

fun main() {
    val dog = Dog()

    dog.eat()
    dog.bark()
}
```

## Override

```kotlin
open class Animal {
    open fun sound() {
        println("Animal sound")
    }
}

class Dog : Animal() {
    override fun sound() {
        println("Woof")
    }
}

fun main() {
    val dog = Dog()

    dog.sound()
}
```

---

# 28. Abstract Classes

```kotlin
abstract class Animal {

    abstract fun sound()

    fun eat() {
        println("Eating")
    }
}

class Dog : Animal() {

    override fun sound() {
        println("Woof")
    }
}

fun main() {
    val dog = Dog()

    dog.sound()
    dog.eat()
}
```

Abstract classes cannot be instantiated directly.

---

# 29. Interfaces

```kotlin
interface Flyable {
    fun fly()
}

class Bird : Flyable {

    override fun fly() {
        println("Bird is flying")
    }
}

fun main() {
    val bird = Bird()

    bird.fly()
}
```

An interface can contain implementation:

```kotlin
interface Logger {

    fun log(message: String) {
        println("LOG: $message")
    }
}

class UserService : Logger

fun main() {
    val service = UserService()

    service.log("User created")
}
```

---

# 30. Data Classes

Data classes are designed for storing data.

```kotlin
data class User(
    val id: Int,
    val name: String,
    val age: Int
)

fun main() {
    val user = User(
        id = 1,
        name = "Heng",
        age = 25
    )

    println(user)
}
```

Data classes automatically provide useful functions such as:

* `toString()`
* `equals()`
* `hashCode()`
* `copy()`
* `componentN()`

## copy

```kotlin
data class User(
    val name: String,
    val age: Int
)

fun main() {
    val user1 = User("Heng", 25)

    val user2 = user1.copy(
        age = 26
    )

    println(user1)
    println(user2)
}
```

---

# 31. Enum Classes

```kotlin
enum class Status {
    PENDING,
    APPROVED,
    REJECTED
}

fun main() {
    val status = Status.APPROVED

    println(status)
}
```

Using `when`:

```kotlin
fun printStatus(status: Status) {
    when (status) {
        Status.PENDING -> println("Waiting")
        Status.APPROVED -> println("Approved")
        Status.REJECTED -> println("Rejected")
    }
}
```

---

# 32. Sealed Classes

Sealed classes are useful when you have a limited set of possible states.

```kotlin
sealed class Result {

    data class Success(
        val data: String
    ) : Result()

    data class Error(
        val message: String
    ) : Result()

    data object Loading : Result()
}

fun handleResult(result: Result) {

    when (result) {

        is Result.Success -> {
            println("Data: ${result.data}")
        }

        is Result.Error -> {
            println("Error: ${result.message}")
        }

        Result.Loading -> {
            println("Loading...")
        }
    }
}

fun main() {
    handleResult(
        Result.Success("Hello Kotlin")
    )

    handleResult(
        Result.Error("Something went wrong")
    )

    handleResult(Result.Loading)
}
```

Sealed classes are especially useful for representing UI states and API results.

---

# 33. Objects and Singleton

Kotlin provides `object` for singleton objects.

```kotlin
object Database {

    fun connect() {
        println("Database connected")
    }
}

fun main() {
    Database.connect()
}
```

There is only one instance of `Database`.

---

# 34. Companion Objects

Companion objects provide class-level members.

```kotlin
class User private constructor(
    val name: String
) {

    companion object {

        fun create(name: String): User {
            return User(name)
        }
    }
}

fun main() {
    val user = User.create("Heng")

    println(user.name)
}
```

---

# 35. Extension Functions

Extension functions allow you to add functionality to an existing type.

```kotlin
fun String.greet(): String {
    return "Hello, $this"
}

fun main() {
    val name = "Heng"

    println(name.greet())
}
```

Another example:

```kotlin
fun Int.isEven(): Boolean {
    return this % 2 == 0
}

fun main() {
    println(10.isEven())
}
```

---

# 36. Scope Functions

Kotlin provides:

* `let`
* `run`
* `with`
* `apply`
* `also`

## let

```kotlin
fun main() {

    val name = "Heng"

    name.let {
        println("Name: $it")
    }
}
```

## apply

`apply` returns the receiver object.

```kotlin
data class User(
    var name: String = "",
    var age: Int = 0
)

fun main() {

    val user = User().apply {
        name = "Heng"
        age = 25
    }

    println(user)
}
```

## also

Useful for side effects such as logging.

```kotlin
fun main() {

    val user = User(
        name = "Heng",
        age = 25
    ).also {
        println("Created user: $it")
    }

    println(user)
}
```

---

# 37. Lambdas

A lambda is an anonymous function.

```kotlin
fun main() {

    val sum = { a: Int, b: Int ->
        a + b
    }

    println(sum(10, 20))
}
```

Output:

```text
30
```

---

# 38. Higher-Order Functions

A higher-order function takes another function as a parameter or returns a function.

```kotlin
fun calculate(
    a: Int,
    b: Int,
    operation: (Int, Int) -> Int
): Int {
    return operation(a, b)
}

fun main() {

    val result = calculate(10, 20) { a, b ->
        a + b
    }

    println(result)
}
```

Another example:

```kotlin
fun executeAction(action: () -> Unit) {
    println("Before")
    action()
    println("After")
}

fun main() {

    executeAction {
        println("Hello Kotlin")
    }
}
```

---

# 39. Generics

Generics allow classes and functions to work with different types.

```kotlin
class Box<T>(
    val value: T
)

fun main() {

    val intBox = Box(100)
    val stringBox = Box("Hello")

    println(intBox.value)
    println(stringBox.value)
}
```

Generic function:

```kotlin
fun <T> printValue(value: T) {
    println(value)
}

fun main() {
    printValue(100)
    printValue("Hello")
    printValue(true)
}
```

---

# 40. Variance

Kotlin supports:

* `out`
* `in`

## out

`out` means the type is produced.

```kotlin
interface Producer<out T> {
    fun produce(): T
}
```

## in

`in` means the type is consumed.

```kotlin
interface Consumer<in T> {
    fun consume(value: T)
}
```

This becomes especially important when designing reusable generic APIs.

---

# 41. Exception Handling

```kotlin
fun main() {

    try {

        val number = "abc".toInt()

        println(number)

    } catch (e: NumberFormatException) {

        println("Invalid number")

    } finally {

        println("Finished")
    }
}
```

## try as expression

```kotlin
fun main() {

    val number = try {
        "123".toInt()
    } catch (e: NumberFormatException) {
        0
    }

    println(number)
}
```

---

# 42. Custom Exceptions

```kotlin
class InvalidAgeException(
    message: String
) : Exception(message)

fun validateAge(age: Int) {

    if (age < 18) {
        throw InvalidAgeException(
            "Age must be at least 18"
        )
    }
}

fun main() {

    try {

        validateAge(15)

    } catch (e: InvalidAgeException) {

        println(e.message)
    }
}
```

---

# 43. File Handling

Kotlin provides convenient file APIs.

```kotlin
import java.io.File

fun main() {

    val file = File("example.txt")

    file.writeText("Hello Kotlin")

    println(file.readText())
}
```

Append:

```kotlin
import java.io.File

fun main() {

    val file = File("example.txt")

    file.appendText("\nSecond line")

    println(file.readText())
}
```

For production applications, consider resource management and appropriate I/O abstractions.

---

# 44. Equality

Kotlin has two important equality operators.

## Structural equality

```kotlin
a == b
```

Checks values.

## Referential equality

```kotlin
a === b
```

Checks whether two references point to the same object.

Example:

```kotlin
fun main() {

    val a = "Hello"
    val b = "Hello"

    println(a == b)
    println(a === b)
}
```

Use `==` for normal value comparison.

---

# 45. Destructuring

Data classes support destructuring.

```kotlin
data class User(
    val name: String,
    val age: Int
)

fun main() {

    val user = User(
        name = "Heng",
        age = 25
    )

    val (name, age) = user

    println(name)
    println(age)
}
```

Destructuring pairs:

```kotlin
fun main() {

    val user = "Heng" to 25

    val (name, age) = user

    println(name)
    println(age)
}
```

---

# 46. Operator Overloading

Kotlin allows operators to be implemented using special functions.

```kotlin
data class Point(
    val x: Int,
    val y: Int
) {

    operator fun plus(other: Point): Point {
        return Point(
            x + other.x,
            y + other.y
        )
    }
}

fun main() {

    val p1 = Point(10, 20)
    val p2 = Point(5, 5)

    val result = p1 + p2

    println(result)
}
```

Output:

```text
Point(x=15, y=25)
```

---

# 47. Delegation

Kotlin supports delegation using `by`.

```kotlin
interface Printer {
    fun print()
}

class ConsolePrinter : Printer {

    override fun print() {
        println("Printing...")
    }
}

class Document(
    printer: Printer
) : Printer by printer

fun main() {

    val document = Document(
        ConsolePrinter()
    )

    document.print()
}
```

Delegation helps reduce boilerplate and composition is often preferable to deep inheritance.

---

# 48. Lazy Initialization

`lazy` delays initialization until the value is first accessed.

```kotlin
val databaseConnection by lazy {

    println("Connecting to database...")

    "Database Connection"
}

fun main() {

    println("Application started")

    println(databaseConnection)

    println(databaseConnection)
}
```

The initializer runs only once.

---

# 49. lateinit

`lateinit` allows a non-null mutable property to be initialized later.

```kotlin
class UserService {

    lateinit var name: String

    fun setup() {
        name = "Heng"
    }

    fun printName() {
        println(name)
    }
}

fun main() {

    val service = UserService()

    service.setup()

    service.printName()
}
```

Do not access a `lateinit` property before initialization.

---

# 50. Inline Functions

`inline` can reduce overhead associated with higher-order functions in appropriate situations.

```kotlin
inline fun measure(block: () -> Unit) {

    val start = System.currentTimeMillis()

    block()

    val end = System.currentTimeMillis()

    println("Time: ${end - start} ms")
}

fun main() {

    measure {
        println("Hello Kotlin")
    }
}
```

Do not use `inline` automatically. Use it when there is a good reason.

---

# 51. Reified Types

A reified type parameter allows access to the generic type at runtime inside an inline function.

```kotlin
inline fun <reified T> printType(value: T) {

    println(T::class.simpleName)
    println(value)
}

fun main() {

    printType(100)
    printType("Hello")
    printType(true)
}
```

Output conceptually:

```text
Int
100
String
Hello
Boolean
true
```

---

# 52. Coroutines

Coroutines are Kotlin's mechanism for writing asynchronous and concurrent code in a structured way.

A common library is `kotlinx.coroutines`.

Example dependency:

```kotlin
dependencies {
    implementation("org.jetbrains.kotlinx:kotlinx-coroutines-core:<version>")
}
```

Example:

```kotlin
import kotlinx.coroutines.delay
import kotlinx.coroutines.launch
import kotlinx.coroutines.runBlocking

fun main() = runBlocking {

    launch {

        delay(1000)

        println("Coroutine finished")
    }

    println("Main continues")
}
```

### Important

Coroutines are not simply "threads".

A coroutine can suspend without blocking the underlying thread.

---

# 53. Suspend Functions

A `suspend` function can suspend execution without blocking the thread.

```kotlin
import kotlinx.coroutines.delay
import kotlinx.coroutines.runBlocking

suspend fun fetchData(): String {

    delay(1000)

    return "Data loaded"
}

fun main() = runBlocking {

    val data = fetchData()

    println(data)
}
```

### Khmer

`suspend` function អាចផ្អាក execution បាន ដោយមិនចាំបាច់ block thread។

វាសំខាន់ណាស់សម្រាប់ network requests, database operations និង asynchronous work។

---

# 54. Coroutine Dispatchers

Common dispatchers:

* `Dispatchers.Default`
* `Dispatchers.IO`
* `Dispatchers.Main`

Example:

```kotlin
import kotlinx.coroutines.Dispatchers
import kotlinx.coroutines.launch
import kotlinx.coroutines.runBlocking

fun main() = runBlocking {

    launch(Dispatchers.Default) {

        println(
            "Running on Default dispatcher"
        )
    }

    launch(Dispatchers.IO) {

        println(
            "Running on IO dispatcher"
        )
    }
}
```

General idea:

### Default

CPU-intensive work.

### IO

Blocking I/O operations.

### Main

UI thread where supported by the platform.

---

# 55. Structured Concurrency

Coroutines should normally have a clear lifecycle.

```kotlin
import kotlinx.coroutines.delay
import kotlinx.coroutines.launch
import kotlinx.coroutines.runBlocking

fun main() = runBlocking {

    launch {
        delay(500)
        println("Task 1")
    }

    launch {
        delay(1000)
        println("Task 2")
    }

    println("Parent waiting for children")
}
```

The child coroutines belong to the parent scope.

This helps avoid uncontrolled background work.

---

# 56. Flow

`Flow` represents an asynchronous stream of values.

```kotlin
import kotlinx.coroutines.delay
import kotlinx.coroutines.flow.Flow
import kotlinx.coroutines.flow.flow
import kotlinx.coroutines.runBlocking

fun numbers(): Flow<Int> = flow {

    for (i in 1..5) {

        delay(500)

        emit(i)
    }
}

fun main() = runBlocking {

    numbers().collect { value ->

        println("Received: $value")
    }
}
```

Concept:

```text
Producer
   |
   v
 Flow
   |
   v
Collector
```

Flow is useful for:

* API streams
* Database changes
* UI state
* Reactive data
* Events

---

# 57. Channels

Channels allow communication between coroutines.

```kotlin
import kotlinx.coroutines.channels.Channel
import kotlinx.coroutines.launch
import kotlinx.coroutines.runBlocking

fun main() = runBlocking {

    val channel = Channel<Int>()

    launch {

        for (i in 1..5) {

            channel.send(i)
        }

        channel.close()
    }

    for (value in channel) {

        println("Received: $value")
    }
}
```

Use channels when you specifically need coroutine-to-coroutine communication.

---

# 58. Generics + Constraints

You can restrict generic types.

```kotlin
fun <T : Number> doubleValue(value: T): Double {

    return value.toDouble() * 2
}

fun main() {

    println(doubleValue(10))
    println(doubleValue(10.5))
}
```

Here `T` must be a subtype of `Number`.

---

# 59. DSL Concepts

Kotlin has language features that make DSL-style APIs possible.

Example:

```kotlin
class HtmlBuilder {

    fun html(block: HtmlBuilder.() -> Unit) {

        println("<html>")

        this.block()

        println("</html>")
    }

    fun body(block: HtmlBuilder.() -> Unit) {

        println("<body>")

        this.block()

        println("</body>")
    }

    fun text(value: String) {

        println(value)
    }
}

fun main() {

    val builder = HtmlBuilder()

    builder.html {

        body {

            text("Hello Kotlin")
        }
    }
}
```

DSL techniques are used by many Kotlin libraries and frameworks.

---

# 60. Advanced Kotlin Project Structure

A larger Kotlin backend project might use a structure like:

```text
src/
└── main/
    └── kotlin/
        └── com/
            └── example/
                ├── Application.kt
                │
                ├── controller/
                │   └── UserController.kt
                │
                ├── service/
                │   └── UserService.kt
                │
                ├── repository/
                │   └── UserRepository.kt
                │
                ├── model/
                │   └── User.kt
                │
                ├── dto/
                │   └── UserDto.kt
                │
                ├── exception/
                │   └── GlobalExceptionHandler.kt
                │
                └── config/
                    └── DatabaseConfig.kt
```

A common architecture is:

```text
Client
  |
  v
Controller
  |
  v
Service
  |
  v
Repository
  |
  v
Database
```

### Khmer

Architecture នេះបែងចែក responsibility របស់ code ជាផ្នែកៗ ដើម្បីធ្វើឱ្យ project ងាយថែទាំ និងពង្រីក។

---

# 61. Best Practices

## 1. Prefer val

Good:

```kotlin
val name = "Heng"
```

Only use `var` when mutation is necessary.

---

## 2. Avoid unnecessary !!

Avoid:

```kotlin
val length = name!!.length
```

Prefer:

```kotlin
val length = name?.length
```

or:

```kotlin
val length = name?.length ?: 0
```

---

## 3. Use data classes for data

Good:

```kotlin
data class User(
    val id: Int,
    val name: String
)
```

---

## 4. Prefer immutable collections

Prefer:

```kotlin
val users = listOf(
    "Heng",
    "Dara"
)
```

over mutable collections when mutation is unnecessary.

---

## 5. Keep functions small

Instead of one giant function:

```kotlin
fun processEverything() {
    // hundreds of lines
}
```

Prefer:

```kotlin
fun validateUser() {
}

fun saveUser() {
}

fun sendNotification() {
}
```

---

## 6. Use meaningful names

Bad:

```kotlin
val x = 100
```

Better:

```kotlin
val maximumUsers = 100
```

---

## 7. Prefer composition

Instead of creating very deep inheritance hierarchies, use interfaces and composition when appropriate.

---

## 8. Avoid unnecessary scope functions

Do not use:

```kotlin
user
    .let {
        it.name
    }
```

when this is enough:

```kotlin
user.name
```

Kotlin's concise syntax should improve readability, not make code harder to understand.

---

# 62. Learning Roadmap

## 🟢 Beginner

Learn these first:

```text
Kotlin syntax
    ↓
Variables
    ↓
Data types
    ↓
Operators
    ↓
Input / Output
    ↓
if / else
    ↓
when
    ↓
Loops
    ↓
Functions
    ↓
Null safety
    ↓
Arrays
    ↓
Collections
```

---

## 🟡 Intermediate

Next learn:

```text
Classes
    ↓
Constructors
    ↓
Properties
    ↓
Inheritance
    ↓
Interfaces
    ↓
Data classes
    ↓
Enums
    ↓
Sealed classes
    ↓
Objects
    ↓
Extension functions
    ↓
Lambdas
    ↓
Higher-order functions
    ↓
Generics
    ↓
Exceptions
```

---

## 🔴 Advanced

Then learn:

```text
Delegation
    ↓
Variance
    ↓
Inline functions
    ↓
Reified types
    ↓
DSL design
    ↓
Coroutines
    ↓
Suspend functions
    ↓
Dispatchers
    ↓
Structured concurrency
    ↓
Flow
    ↓
Channels
    ↓
Concurrency patterns
    ↓
Architecture
    ↓
Testing
    ↓
Performance
```

---

# 🚀 What to Learn After Kotlin

Once you understand the Kotlin language, choose a direction.

## Android

```text
Kotlin
  ↓
Android
  ↓
Jetpack Compose
  ↓
Room
  ↓
Retrofit
  ↓
Coroutines
  ↓
Flow
  ↓
Clean Architecture
```

## Backend

```text
Kotlin
  ↓
HTTP
  ↓
REST API
  ↓
Ktor or Spring Boot
  ↓
Database
  ↓
JPA / Hibernate
  ↓
Authentication
  ↓
JWT
  ↓
Testing
  ↓
Docker
  ↓
Deployment
```

## Multiplatform

```text
Kotlin
  ↓
Kotlin Multiplatform
  ↓
Shared Business Logic
  ↓
Android
  +
iOS
  +
Desktop
```

---

# 🧪 Practice Project Ideas

## Beginner

### 1. Calculator

Features:

```text
Addition
Subtraction
Multiplication
Division
```

### 2. Number Guessing Game

Features:

```text
Random number
User input
Attempts
Win / Lose
```

### 3. Student Grade System

Features:

```text
Student name
Scores
Average
Grade
```

---

# 🟡 Intermediate Projects

### 4. Todo Application

Features:

```text
Create todo
Read todos
Update todo
Delete todo
Mark completed
Search
Filter
```

### 5. Banking Application

Features:

```text
Create account
Deposit
Withdraw
Transfer
Transaction history
Balance
```

### 6. Inventory System

Features:

```text
Products
Categories
Stock
Purchase
Sale
Search
Reports
```

---

# 🔴 Advanced Projects

### 7. REST API

Build:

```text
Authentication
Users
Products
Orders
Payments
Database
Validation
Exception handling
Logging
Testing
```

Architecture:

```text
Controller
     ↓
Service
     ↓
Repository
     ↓
Database
```

---

# 🏆 Final Kotlin Skill Map

```text
                         KOTLIN
                            |
          ┌─────────────────┼─────────────────┐
          |                 |                 |
       Basics             OOP             Functional
          |                 |                 |
     Variables          Classes            Lambda
     Types              Objects            map
     Conditions         Inheritance        filter
     Loops              Interface          reduce
     Functions          Data Class         fold
          |                 |                 |
          └─────────────────┼─────────────────┘
                            |
                       Advanced Kotlin
                            |
          ┌─────────────────┼─────────────────┐
          |                 |                 |
       Generics         Delegation        Extensions
          |                 |                 |
       Variance          by                DSL
          |                 |                 |
          └─────────────────┼─────────────────┘
                            |
                       Coroutines
                            |
          ┌─────────────────┼─────────────────┐
          |                 |                 |
       Suspend           Flow             Channel
       Dispatchers       StateFlow        Concurrency
       Scope             SharedFlow        Async
          |                 |                 |
          └─────────────────┼─────────────────┘
                            |
                         Projects
                            |
          ┌─────────────────┼─────────────────┐
          |                 |                 |
       Android           Backend         Multiplatform
          |                 |                 |
     Compose             Ktor          Kotlin Multiplatform
     Room                Spring Boot
     Retrofit            Database
```

---

# 🎯 Final Advice

Do not try to memorize all Kotlin syntax.

Instead:

```text
Learn
 ↓
Understand
 ↓
Write code
 ↓
Make mistakes
 ↓
Debug
 ↓
Build projects
 ↓
Read other people's code
 ↓
Build larger projects
```

The most important progression is:

```text
Kotlin Basics
      ↓
Object-Oriented Programming
      ↓
Functional Programming
      ↓
Collections
      ↓
Generics
      ↓
Null Safety
      ↓
Coroutines
      ↓
Flow
      ↓
Testing
      ↓
Architecture
      ↓
Real Projects
```

If you master those areas, you will have a strong foundation for professional Kotlin development.
