# KOTLIN

* IntelliJ IDEA의 개발사 JetBrains에서 2011년에 공개한 프로그래밍 언어. 간결한 문법을 가지고 있으며, 세미콜론은 옵션이다. JVM 기반의 언어이며, Java와의 상호 운용이 100% 지원된다. JVM 바이트코드가 기본이지만, Kotlin/Native 컴파일러를 사용하여 기계어로 최종컴파일이 가능하다. 안드로이드, 톰캣[1], JavaScript, Java EE, HTML5, iOS, 라즈베리 파이 등을 개발할 때 사용할 수 있다. 현재 공식 1.2.60 버전이 나와 있다

*
kotlinlang.org/kotlin_250x250.png

```kotlin
package hello

fun main(args: Array<String>) {
   println("Hello World!")
}
```

## kotlin's

* new 키워드가 없다.
 * 세미콜론이 필요없다.
 * System.out.println/printf 등이 println/printf 등으로 줄었다.
 * String에서 변수의 값을 쉽게 표현할 수 있는 interpolation($)을 지원한다.
{{{#!html
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">val</span> name: String = <span style="background-color: #fff0f0">"Wikineet"</span>
<span style="color: #008800; font-weight: bold">val</span> greet_en: String = <span style="background-color: #fff0f0">"Hello, $name!"</span>
<span style="color: #008800; font-weight: bold">val</span> greet_ko: String = <span style="background-color: #fff0f0">"${name}님 안녕하세요!"</span>
println(greet_en) <span style="color: #888888">// 출력: Hello, Wikineet!</span>
println(greet_ko) <span style="color: #888888">// 출력: Wikineet님 안녕하세요!</span>
</pre></div>
}}}
 * Nullable이 아닌 변수에서 null 사용시 오류를 뱉어낸다.
{{{#!html <!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%">var a: String <span style="color: #333333">=</span> <span style="background-color: #fff0f0">"abc"</span>
a <span style="color: #333333">=</span> null <span style="color: #333333">//</span> 컴파일 에러
</pre></div>
}}}
  * ?을 사용해 Nullable로 만들어주면 쓸 수 있다.
{{{#!html <!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">var</span> b: String? = <span style="background-color: #fff0f0">"abc"</span>
b = <span style="color: #008800; font-weight: bold">null</span> <span style="color: #888888">// ok</span></pre></div>
}}}
  * Elvis 연산자(?:)가 존재한다.
{{{#!html
<!-- HTML generated using hilite.me --><div style="background: #ffffff; overflow:auto;width:auto;border:solid gray;border-width:.1em .1em .1em .8em;padding:.2em .6em;"><pre style="margin: 0; line-height: 125%"><span style="color: #008800; font-weight: bold">val</span> testee_hometown: String? = <span style="color: #008800; font-weight: bold">null</span> <span style="color: #888888">// 여기에 적절한 값을 넣으면 '<피실험자 고향 지명>' 대신 넣은 값이 표시된다.</span>
<span style="color: #008800; font-weight: bold">val</span> hometown_display = testee_hometown ?: <span style="background-color: #fff0f0">"<피실험자 고향 지명>"</span> <span style="color: #888888">// testee_hometown이 null인지 검사한다. null이면 연산자의 우변에 있는 값이 대신 대입된다.</span>
println(<span style="background-color: #fff0f0">"이 장치는 ${hometown_display}에 사는 모든 사람의 신체 장기 가격과 소득 금액을 합친 것보다 더 비쌉니다."</span>)
</pre></div>
}}}

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

