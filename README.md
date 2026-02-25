## Java Core Concepts

1. String, Date, Time and Numeric objects.
    - 1.1. [StringBuilder class.](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/StringBuilder.html)
    - 1.2. [Date and Time.](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/time/package-summary.html)
    - 1.3. [BigDecimal class.](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/math/BigDecimal.html)
2. [Object class (equals, hashCode, toString).](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Object.html#equals(java.lang.Object))
    - 2.1. [Objects class.](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Objects.html)
3. [Enum classes.](https://docs.oracle.com/javase/specs/jls/se17/html/jls-8.html#jls-8.9)
4. [Record classes.](https://docs.oracle.com/javase/specs/jls/se17/html/jls-8.html#jls-8.10)
5. [Sealed classes.](https://docs.oracle.com/javase/specs/jls/se17/html/jls-8.html#jls-8.1.1.2)
6. [Optional.](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Optional.html)
7. [Exceptions.](https://docs.oracle.com/javase/specs/jls/se17/html/jls-11.html)
8. [Generic classes and Type Parameters.](https://docs.oracle.com/javase/specs/jls/se17/html/jls-8.html#jls-8.1.2)
9. [Collection.](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collection.html)
    - 9.1. [Collections class.](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/Collections.html)
10. I/O and NIO
    - 10.1. [I/O](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/io/package-summary.html)
    - 10.2. [NIO](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/nio/package-summary.html)
    - 10.3. [NIO File](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/nio/file/package-summary.html)
11. JDBC
    - 11.1. [Driver.](https://docs.oracle.com/en/java/javase/17/docs/api/java.sql/java/sql/Driver.html)
    - 11.2. [Connection.](https://docs.oracle.com/en/java/javase/17/docs/api/java.sql/java/sql/Connection.html)
    - 11.3. [Statement.](https://docs.oracle.com/en/java/javase/17/docs/api/java.sql/java/sql/Statement.html)
    - 11.4. [PreparedStatement.](https://docs.oracle.com/en/java/javase/17/docs/api/java.sql/java/sql/PreparedStatement.html)
    - 11.5. [CallableStatement.](https://docs.oracle.com/en/java/javase/17/docs/api/java.sql/java/sql/CallableStatement.html)
    - 11.6. [ResultSet.](https://docs.oracle.com/en/java/javase/17/docs/api/java.sql/java/sql/ResultSet.html)
    - 11.7. [DataSource.](https://docs.oracle.com/en/java/javase/17/docs/api/java.sql/javax/sql/DataSource.html)
12. [Functional Interfaces.](https://docs.oracle.com/javase/specs/jls/se17/html/jls-9.html#jls-9.8)
13. [Lambda Expressions.](https://docs.oracle.com/javase/specs/jls/se17/html/jls-15.html#jls-15.27)
14. [Streams API.](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/stream/package-summary.html)
15. [Concurrency and Multithreading.](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/concurrent/package-summary.html)
    - 15.1. [Thread.](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/Thread.html)
    - 15.2. [Atomic.](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/concurrent/atomic/package-summary.html)
    - 15.3. [Locks.](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/util/concurrent/locks/package-summary.html)
    - 15.4. [Synchronized Methods.](https://docs.oracle.com/javase/specs/jls/se17/html/jls-8.html#jls-8.4.3.6)
    - 15.5. [Threads and Locks.](https://docs.oracle.com/javase/specs/jls/se17/html/jls-17.html)
16. Annotations.
    - 16.1. [Annotation Interfaces.](https://docs.oracle.com/javase/specs/jls/se17/html/jls-9.html#jls-9.6)
    - 16.2. [Annotations.](https://docs.oracle.com/javase/specs/jls/se17/html/jls-9.html#jls-9.7)
17. [Reflections.](https://docs.oracle.com/en/java/javase/17/docs/api/java.base/java/lang/reflect/package-summary.html)

---
## Common Java Questions

- **What is the difference between == and equals()?**
    > *== compares whether two references point to the same object, while equals() compares whether two objects are logically equivalent according to the class’s definition.*
- **Why is String immutable?**
    > *Immutability makes String thread-safe, allows safe reuse in the string pool, enables reliable hashing, and prevents accidental or malicious modification.*
- **How do String, StringBuilder, and StringBuffer differ?**
    > *String is immutable, StringBuilder is mutable and fast but not thread-safe, and StringBuffer is mutable and synchronized, making it thread-safe but slower.*
- **What is an enum and why should it be used in Java?**
    > *An enum is a special type used to define a fixed set of constants with type safety, built-in support for comparison and iteration, and the ability to associate behavior and fields with each constant.*
- **What is the purpose of Optional?**
    > *Optional explicitly represents the presence or absence of a value, reducing null checks and making APIs clearer about whether a result may be missing.*
- **What is the difference between orElse() and orElseGet() in Optional?**
    > *orElse() always evaluates its argument, even when the value is present, while orElseGet() evaluates the supplier lazily and only when the Optional is empty, making it preferable when the fallback computation is expensive or has side effects.*
- **What is the difference between get() and orElseThrow() in Optional?**
    > *get() returns the value or throws a generic NoSuchElementException, whereas orElseThrow() makes the absence explicit and allows supplying a custom exception, resulting in clearer intent and better error handling.*
- **What is the equals() and hashCode() contract?**
    > *If two objects are equal according to equals(), they must return the same hashCode(), otherwise hash-based collections will behave incorrectly.*
- **What is the difference between checked and unchecked exceptions?**
    > *Checked exceptions represent recoverable conditions and must be handled or declared, while unchecked exceptions indicate programming errors and are not enforced by the compiler.*
- **What is a record?**
    > *A record is a concise, immutable data carrier that automatically provides a constructor, accessors, and standard implementations of equals, hashCode, and toString.*
- **What problem do sealed classes solve?**
    > *Sealed classes restrict which types may extend or implement them, enabling controlled inheritance and safer modeling of closed type hierarchies.*
- **What is a functional interface?**
    > *A functional interface has exactly one abstract method, allowing it to be implemented using a lambda expression or method reference.*
- **What is the difference between Collection and Collections?**
    > *Collection is a core interface representing a group of elements, while Collections is a utility class providing static helper methods for working with collections.*
- **What is the difference between map() and flatMap() in streams?**
    > *map() transforms each element individually, while flatMap() transforms and flattens nested structures into a single stream.*
- **How many times can a stream be consumed?**
    > *A stream can be consumed only once, after a terminal operation is executed, the stream is closed and any further use results in an IllegalStateException, which enforces a single-pass, pipeline-based processing model.*
- **What is the difference between HashMap and ConcurrentHashMap?**
    > *HashMap is not thread-safe and can behave unpredictably under concurrent access, while ConcurrentHashMap is designed for concurrency using fine-grained synchronization, allowing safe concurrent reads and updates without locking the entire map.*
- **How does Thread differ from Runnable?**
    > *Thread represents the execution mechanism, while Runnable represents the task to be executed, making Runnable more flexible and reusable.*
- **What does synchronized guarantee?**
    > *synchronized ensures exclusive access to a critical section and establishes memory visibility guarantees defined by the Java Memory Model.*
- **What is a race condition?**
    > *A race condition occurs when multiple threads access shared mutable state without proper coordination, causing results to depend on execution timing.*
- **Why use PreparedStatement instead of Statement?**
    > *PreparedStatement prevents SQL injection, improves performance through precompilation, and supports parameterized queries.*
- **What is reflection used for?**
    > *Reflection allows inspection and interaction with classes, methods, and fields at runtime, enabling frameworks and dynamic behavior.*
- **What are the main Object-Oriented Programming (OOP) principles in Java?**
    > *Java is based on four core OOP principles: Encapsulation, which hides internal state behind controlled access. Abstraction, which exposes behavior while hiding implementation details. Inheritance, which enables reuse by deriving new types from existing ones. And Polymorphism, which allows objects to be treated uniformly while exhibiting different behavior at runtime.*
- **When should composition be preferred over inheritance?**
    > *Composition should be preferred when behavior needs to be reused without tight coupling, as it provides greater flexibility and avoids the fragility of deep inheritance hierarchies.*
- **What is the difference between an interface and an abstract class?**
    > *An interface defines a contract without state and supports multiple inheritance, while an abstract class can hold state and shared implementation but supports only single inheritance.*
- **What is immutability and how does it relate to OOP?**
    > *An immutable object cannot change its state after creation, simplifying reasoning, improving thread safety, and aligning well with encapsulation principles.*
- **What does the final keyword do in Java?**
    > *The final keyword prevents modification: a final variable cannot be reassigned, a final method cannot be overridden, and a final class cannot be extended, helping enforce immutability, prevent unintended behavior changes, and improve program safety.*
- **Can a static method be overridden in Java?**
    > *No, static methods cannot be overridden because they belong to the class rather than the instance. When a subclass declares a static method with the same signature, it hides the parent method, and the method call is resolved at compile time based on the reference type.*
---
References

- [The Java Language Specification (17)](https://docs.oracle.com/javase/specs/jls/se17/html/index.html)

- [The Java Language Documentation (17)](https://docs.oracle.com/en/java/javase/17/docs/api/index.html)
