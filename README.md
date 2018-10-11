# KOTLIN

* IntelliJ IDEA의 개발사 JetBrains에서 2011년에 공개한 프로그래밍 언어. 간결한 문법을 가지고 있으며, 세미콜론은 옵션이다. JVM 기반의 언어이며, Java와의 상호 운용이 100% 지원된다. JVM 바이트코드가 기본이지만, Kotlin/Native 컴파일러를 사용하여 기계어로 최종컴파일이 가능하다. 안드로이드, 톰캣[1], JavaScript, Java EE, HTML5, iOS, 라즈베리 파이 등을 개발할 때 사용할 수 있다. 현재 공식 1.2.60 버전이 나와 있다

*
kotlinlang.org/kotlin_250x250.png

'''kotlin
package hello

fun main(args: Array<String>) {
   println("Hello World!")
}
'''



# kotlin in action

[![official JetBrains project](http://jb.gg/badges/official-plastic.svg)](https://confluence.jetbrains.com/display/ALL/JetBrains+on+GitHub)

This project contains the code samples from the "Kotlin in Action" book (https://www.manning.com/books/kotlin-in-action).
To build the project import it as Gradle project.

Each of the samples is a self-contained file, and most of them contain a "main"
function. To run a sample, simply open the file in the IDE, right-click the
"main" function and select the "Run" or "Debug" option from the context menu.

Some of the samples do not contain a "main" function, and are provided only as
a reference or demonstration of a concept. You can simply study them, or you
can incorporate them into your own examples or exercises.

The numbering of the sample files corresponds to the order in which they
appear in the book.
