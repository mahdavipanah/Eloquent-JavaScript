{{meta {load_files: ["code/intro.js"]}}}

# مقدمه

{{quote {author: "اِلن اولمَن", title: "نزدیک به ماشین: تکنوفیلیا و ناخشنودی‌های آن", chapter: true}
ما فکر می‌کنیم که سیستم را برای اهداف خودمان می‌سازیم. ما گمان می‌کنیم که آن را در تصور خود می‌سازیم... اما رایانه در واقع شبیه
به ما نیست. رایانه تنها نمایی از بخش کوچکی از ماست: همان قسمتی که به منطق، نظم، قانون و شفافیت اختصاص دارد.

quote}}

{{figure {url: "img/chapter_picture_00.jpg", alt: "Picture of a screwdriver and a circuit board", chapter: "framed"}}}

این کتاب درمورد تعلیم دادن کامپیوتر‌ها است. امروزه کامپیوتر‌ها به اندازه‌ی پیچ‌گوشتی‌ها متداول شده‌اند، اما بسیار پیچیده‌تر از
پیچ‌گوشتی‌ها هستند و این که تعلیمشان دهیم تا کاری که ما می‌خواهیم را انجام دهند، همیشه آسان نیست.

اگر وظیفه‌ای که برای کامپیوتر خود تعریف می‌کنید، یک کار معمول و کاملا قابل درک باشد، مثل نمایش دادن ایمیل‌هایتان و یا عمل کردن
شبیه به یک ماشین حساب، آنوقت می‌توانید برنامه‌ی مناسب را باز کنید و کارتان را شروع کنید. اما برای یک تکلیف منحصر به فرد و یا غیر قابل
تعریف و بی‌انتها، به احتمال زیاد برنامه‌ای وجود ندارد.

اینجاست که پای برنامه‌نویسی به وسط می‌آید. برنامه‌نویسی کار  ِ ساخت _برنامه‌هاست_. برنامه شامل دستورات دقیقی است که به کامپیوتر
می‌گوید چه کاری انجام دهد. از آنجا که کامپیوتر‌ها بسیار احمق و البته دقیق هستند و ایرادات ملانقطه‌ای می‌گیرند، برنامه‌نویسی
به طور ذاتی کاری طاقت‌فرساست.

{{index [programming, "joy of"], speed}}

خوش‌بختانه، اگر بتوانید با سختی  ِ فکر کردن به مسائل به گونه‌ای که کامپیوتر‌های احمق برایشان قابل درک است، کنار بیایید،
برنامه‌نویسی می‌تواند برایتان فوق‌العاده لذت‌بخش باشد. این امکان را به تو می‌دهد تا کارهای طولانی و طاقت‌فرسا را در کثری از ثانیه
انجام دهید. این امکان را به تو می‌دهد تا کامپیوترتان را تعلیم دهید تا کارهایی را بکند که قبلا نمی‌توانسته.
و البته یک تمرین فوق‌العاده برای تفکر انتزاعی هم هست.

بیشتر کار برنامه‌نویسی با زبان‌های برنامه‌نویسی انجام می‌شود. یک _زبان برنامه‌نویسی_، یک زبان ساختگی است که از آن برای دادن
دستورات به کامپیوتر استفاده می‌شود. نکته‌ی بسیار جالب این است که، روشی که ما برای ارتباط با کامپیوترها یافته‌ایم
بسیار شبیه به روشی است که خود ما برای ارتباط با یکدیگر استفاده می‌کنیم. مثل زبان‌های انسانی، زبان کامپیوتر این امکان
را به ما می‌دهد که کلمات و عبارات را به گونه‌های جدید باهم ترکیب کنیم و بدین صورت مفاهیم جدیدی را با استفاده از آن‌ها بیان کنیم.

{{index [JavaScript, "availability of"], "casual computing"}}

زمانی بود که رابط‌های مبتنی بر زبان، مثل BASIC و DOS در دهه‌ی ۱۹۸۰ و ۱۹۹۰ میلادی، روش اصلی برای ارتباط با کامپیوتر‌ها
بودند. اما امروزه آن‌ها به طور گسترده‌ای با رابط‌های دیداری جایگزین شده‌اند؛ یادگیری رابط‌های بصری راحت‌تر است اما آزادی عمل کمتری
به ما می‌دهند. اگر بدانید کجا را بگردید، می‌فهمید که زبان‌های برنامه‌نویسی هنوز هم وجود دارند. یکی از این زبان‌ها
جاوااسکریپت است، که درون تمام مرورگر‌های مدرن وب گنجانده شده و بنابراین می‌توان گفت که تقریبا روی هر دستگاهی موجود است.

{{indexsee "web browser", browser}}

این کتاب تلاش دارد تا تو را به اندازه‌ی کافی با این زبان آشنا کند تا بتوانید با آن کار‌های مفید و سرگرم‌کننده بکنید.

## درمورد برنامه‌نویسی

{{index [programming, "difficulty of"]}}

در کنار توضیح جاوااسکریپت، قواعد ابتدایی برنامه‌نویسی را نیز معرفی خواهم کرد. برنامه‌نویسی کار سختی است. اصول پایه‌ای
آن ساده و قابل فهم‌اند، ولی برنامه‌هایی که بر پایه‌ی این قوانین نوشته می‌شوند، پیچیده از آب در می‌آیند و قوانین و دشواری‌های
خاص خود را درست می‌کنند. مثل این است که برای خودت هزارتویی بسازی، چون ممکن است خودت نیز در آن گم شوی.

{{index learning}}

در طی خواندن این کتاب ممکن است در جاهایی ناامید شوید. اگر با برنامه‌نویسی ناآشنا باشید، اطلاعات جدید زیادی را باید هضم
کنید. بسیاری از این اطلاعات دوباره نیز  باهم _ترکیب_ می‌شوند که فهم آن‌ها نیازمند تمرکز دوچندان است.

این به عهده‌ی تو است که به اندازه کافی تلاش کنی. وقتی برای دنبال کردن مفاهیم و فهم آن‌ها در حین خواندن کتاب در حال تقلا
و تلاش هستی، این سختی را به دوش توان و استعداد خود نگذار. تو قطعا به اندازه‌ی کافی قابلیت یادگیری داری و تنها نیاز است که
ادامه دهی. کمی استراحت کن، بعضی مطالب را دوباره بخوان و مطمئن شو که مثال برنامه‌ها و تمرین‌ها را می‌خوانی و کامل درک می‌کنی.
یادگیری کار سختی است، اما هرچه که یاد می‌گیری اندوخته‌ای است برای خودت و یادگیری‌های آتی‌ات را آسان‌تر خواهد کرد.

{{quote {author: "اورسولا کروبر لو گویین", title: "دست چپ تاریکی"}

{{index "Le Guin, Ursula K."}}

وقتی که انجام کار‌ها فایده‌ای ندارد، به جمع کردن اطلاعات بپرداز؛ وقتی اطلاعات هم سودی ندارد، بخواب.

quote}}

{{index [program, "nature of"], data}}

یک برنامه‌ی کامپیوتری، خیلی چیزهاست. یک قطعه از متن است که توسط برنامه‌نویس نوشته‌شده‌است، نیروی هدایت‌کننده‌ای است که باعث
می‌شود کامپیوتر کاری را که باید، بکند، اطلاعاتی است که داخل حافظه‌ی کامپیوتر است، و در عین حال اعمالی که روی همان حافظه
انجام می‌شود را نیز کنترل می‌کند. به نظر می‌رسد مثال‌هایی که تلاش دارند تا برنامه‌های کامپیوتری را با اشیائی که ما با آن‌ها
آشنا هستیم، مقایسه کنند، درک درست و دقیقی نمی‌دهند. یکی از همین قیاس‌ها که می‌تواند درکی کلی به ما بدهد،
برنامه‌ی کامپیوتری را به یک ماشین تشبیه می‌کند، ماشینی که برای این که کار کند از اجزای مجزای زیادی تشکیل شده و برای فهم
طرز کارکرد آن باید رابطه‌ی بین این اجزا و وظایفشان را در نظر بگیریم.

کامپیوتر، ماشینی فیزیک است که  به عنوان میزبانی برای این ماشین‌های غیرمادی (برنامه‌های کامپیوتری) عمل می‌کند.
کامپیوتر‌ها خود به تنهایی قادرند کارهایی بسیار سرراست و احمقانه را انجام دهند. دلیلی که باعث می‌شود کامپیوترها تا این
اندازه مفید باشند، این است که همین کارهای بسیار ساده را فوق‌العاده سریع انجام می‌دهند. یک برنامه‌ی کامپیوتری می‌تواند
به طور هوشمندانه‌ای از ترکیب بی‌شماری از همین کارهای ساده تشکیل شده و انجام کارهایی بسیار پیچیده را ممکن کند.

{{index [programming, "joy of"]}}

یک برنامه‌های کامپیوتری، سازه‌ای از تفکرات است. درست‌کردنش بدون‌هزینه‌است، وزنی ندارد و تنها با انگشتانی که قادر به تایپ
هستند قابل ساخت است.

اگر دقت کافی نشود، اندازه و پیچیدگی یک برنامه‌ی کامپیوتری می‌تواند از کنترل خارج شود و حتی شخصی که آن را نوشته را نیز
دچار سردرگمی کند. مسئله‌ی اصلی در برنامه‌نویسی، تحت کنترل نگه داشتن برنامه‌های کامپیوتری است. وقتی یک برنامه کار می‌کند، بسیار
زیباست. هنر برنامه‌نویسی، مهارت در کنترل کردن پیچیدگی است. یک برنامه‌ی عالی، برنامه‌ای مهار شده است - با تمام پیچیدگی‌ای
که دارد، ساده نوشته‌شده‌است.

{{index "programming style", "best practices"}}

بعضی از برنامه‌نویس‌ها گمان می‌کنند بهترین راه برای مدیریت این پیچیدگی، استفاده از مجموعه‌ی کوچکی از تکنیک‌های به خوبی درک
شده در برنامه‌ها است. آن‌ها قواعد سرسختی را وضع‌کرده‌اند («تجربه‌ی برتر») که شکل و فرم برنامه‌ها را وضع می‌کند و برنامه‌ها را
در یک محدوده‌ی امن و کوچک خودشان نگه می‌دارد.

{{index experiment}}

این کار نه تنها کسالت‌بار است، بلکه بی‌فایده هم هست. مسائل جدید اغلب نیازمند راه‌حل‌هایی جدید هستند. رشته‌ی برنامه‌نویسی هنوز
جوان است و به سرعت در حال پیشرفت است و به اندازه‌ی کافی متنوع هست که جا برای مجموعه‌ی گسترده‌ای از رویکرد‌های گوناگون
را داشته باشد. اشتباهات مهلک زیادی هست که در طراحی برنامه‌های کامپیوتری وجود دارد و بهترین راه برای درک درست و کامل آن‌ها،
به جلو رفتن، مرتکب آن‌ها شدن و تجربه‌کردنشان است. حس تشخیص یک برنامه‌ی خوب از بد، نه از لیستی از قوانین، که با  تمرین و
ممارست به وجود می‌آید.

## Why language matters

{{index "programming language", "machine code", "binary data"}}

In the beginning, at the birth of computing, there were no programming
languages. Programs looked something like this:

```{lang: null}
00110001 00000000 00000000
00110001 00000001 00000001
00110011 00000001 00000010
01010001 00001011 00000010
00100010 00000010 00001000
01000011 00000001 00000000
01000001 00000001 00000001
00010000 00000010 00000000
01100010 00000000 00000000
```

{{index [programming, "history of"], "punch card", complexity}}

That is a program to add the numbers from 1 to 10 together and print
out the result: `1 + 2 + ... + 10 = 55`. It could run on a simple,
hypothetical machine. To program early computers, it was necessary to
set large arrays of switches in the right position or punch holes in
strips of cardboard and feed them to the computer. You can probably
imagine how tedious and error-prone this procedure was. Even writing
simple programs required much cleverness and discipline. Complex ones
were nearly inconceivable.

{{index bit, "wizard (mighty)"}}

Of course, manually entering these arcane patterns of bits (the ones
and zeros) did give the programmer a profound sense of being a mighty
wizard. And that has to be worth something in terms of job
satisfaction.

{{index memory, instruction}}

Each line of the previous program contains a single instruction. It
could be written in English like this:

 1. Store the number 0 in memory location 0.
 2. Store the number 1 in memory location 1.
 3. Store the value of memory location 1 in memory location 2.
 4. Subtract the number 11 from the value in memory location 2.
 5. If the value in memory location 2 is the number 0,
    continue with instruction 9.
 6. Add the value of memory location 1 to memory location 0.
 7. Add the number 1 to the value of memory location 1.
 8. Continue with instruction 3.
 9. Output the value of memory location 0.

{{index readability, naming, binding}}

Although that is already more readable than the soup of bits, it is
still rather obscure. Using names instead of numbers for the
instructions and memory locations helps.

```{lang: "text/plain"}
 Set “total” to 0.
 Set “count” to 1.
[loop]
 Set “compare” to “count”.
 Subtract 11 from “compare”.
 If “compare” is zero, continue at [end].
 Add “count” to “total”.
 Add 1 to “count”.
 Continue at [loop].
[end]
 Output “total”.
```

{{index loop, jump, "summing example"}}

Can you see how the program works at this point? The first two lines
give two memory locations their starting values: `total` will be used
to build up the result of the computation, and `count` will keep track
of the number that we are currently looking at. The lines using
`compare` are probably the weirdest ones. The program wants to see
whether `count` is equal to 11 to decide whether it can stop
running. Because our hypothetical machine is rather primitive, it can
only test whether a number is zero and make a decision based
on that. So it uses the memory location labeled `compare` to compute
the value of `count - 11` and makes a decision based on that value.
The next two lines add the value of `count` to the result and
increment `count` by 1 every time the program has decided that `count`
is not 11 yet.

Here is the same program in JavaScript:

```
let total = 0, count = 1;
while (count <= 10) {
  total += count;
  count += 1;
}
console.log(total);
// → 55
```

{{index "while loop", loop, [braces, block]}}

This version gives us a few more improvements. Most important, there
is no need to specify the way we want the program to jump back and
forth anymore. The `while` construct takes care of that. It continues
executing the block (wrapped in braces) below it as long as the
condition it was given holds. That condition is `count <= 10`, which
means “_count_ is less than or equal to 10”. We no longer have to
create a temporary value and compare that to zero, which was just an
uninteresting detail. Part of the power of programming languages is
that they can take care of uninteresting details for us.

{{index "console.log"}}

At the end of the program, after the `while` construct has finished,
the `console.log` operation is used to write out the result.

{{index "sum function", "range function", abstraction, function}}

Finally, here is what the program could look like if we happened to
have the convenient operations `range` and `sum` available, which
respectively create a ((collection)) of numbers within a range and
compute the sum of a collection of numbers:

```{startCode: true}
console.log(sum(range(1, 10)));
// → 55
```

{{index readability}}

The moral of this story is that the same program can be expressed in
both long and short, unreadable and readable ways. The first version of the
program was extremely obscure, whereas this last one is almost
English: `log` the `sum` of the `range` of numbers from 1 to 10. (We
will see in [later chapters](data) how to define operations like `sum`
and `range`.)

{{index ["programming language", "power of"], composability}}

A good programming language helps the programmer by allowing them to
talk about the actions that the computer has to perform on a higher
level. It helps omit details, provides convenient building blocks
(such as `while` and `console.log`), allows you to define your own
building blocks (such as `sum` and `range`), and makes those blocks
easy to compose.

## What is JavaScript?

{{index history, Netscape, browser, "web application", JavaScript, [JavaScript, "history of"], "World Wide Web"}}

{{indexsee WWW, "World Wide Web"}}

{{indexsee Web, "World Wide Web"}}

JavaScript was introduced in 1995 as a way to add programs to web
pages in the Netscape Navigator browser. The language has since been
adopted by all other major graphical web browsers. It has made modern
web applications possible—applications with which you can interact
directly without doing a page reload for every action. JavaScript is also
used in more traditional websites to provide various forms of
interactivity and cleverness.

{{index Java, naming}}

It is important to note that JavaScript has almost nothing to do with
the programming language named Java. The similar name was inspired by
marketing considerations rather than good judgment. When JavaScript
was being introduced, the Java language was being heavily marketed and
was gaining popularity. Someone thought it was a good idea to try to
ride along on this success. Now we are stuck with the name.

{{index ECMAScript, compatibility}}

After its adoption outside of Netscape, a ((standard)) document was
written to describe the way the JavaScript language should work so
that the various pieces of software that claimed to support JavaScript
were actually talking about the same language. This is called the
ECMAScript standard, after the Ecma International organization that
did the standardization. In practice, the terms ECMAScript and
JavaScript can be used interchangeably—they are two names for the same
language.

{{index [JavaScript, "weaknesses of"], debugging}}

There are those who will say _terrible_ things about JavaScript. Many
of these things are true. When I was required to write something in
JavaScript for the first time, I quickly came to despise it. It would
accept almost anything I typed but interpret it in a way that was
completely different from what I meant. This had a lot to do with the
fact that I did not have a clue what I was doing, of course, but there
is a real issue here: JavaScript is ridiculously liberal in what it
allows. The idea behind this design was that it would make programming
in JavaScript easier for beginners. In actuality, it mostly makes
finding problems in your programs harder because the system will not
point them out to you.

{{index [JavaScript, "flexibility of"], flexibility}}

This flexibility also has its advantages, though. It leaves space for
a lot of techniques that are impossible in more rigid languages, and
as you will see (for example in [Chapter ?](modules)), it can be used
to overcome some of JavaScript's shortcomings. After ((learning)) the
language properly and working with it for a while, I have learned to
actually _like_ JavaScript.

{{index future, [JavaScript, "versions of"], ECMAScript, "ECMAScript 6"}}

There have been several versions of JavaScript. ECMAScript version 3
was the widely supported version in the time of JavaScript's ascent to
dominance, roughly between 2000 and 2010. During this time, work was
underway on an ambitious version 4, which planned a number of radical
improvements and extensions to the language. Changing a living, widely
used language in such a radical way turned out to be politically
difficult, and work on the version 4 was abandoned in 2008, leading to
a much less ambitious version 5, which made only some uncontroversial
improvements, coming out in 2009. Then in 2015 version 6 came out, a
major update that included some of the ideas planned for version 4.
Since then we've had new, small updates every year.

The fact that the language is evolving means that browsers have to
constantly keep up, and if you're using an older browser, it may not
support every feature. The language designers are careful to not make
any changes that could break existing programs, so new browsers can
still run old programs. In this book, I'm using the 2017 version of
JavaScript.

{{index [JavaScript, "uses of"]}}

Web browsers are not the only platforms on which JavaScript is used.
Some databases, such as MongoDB and CouchDB, use JavaScript as their
scripting and query language. Several platforms for desktop and server
programming, most notably the ((Node.js)) project (the subject of
[Chapter ?](node)), provide an environment for programming JavaScript
outside of the browser.

## Code, and what to do with it

{{index "reading code", "writing code"}}

_Code_ is the text that makes up programs. Most chapters in this book
contain quite a lot of code. I believe reading code and writing ((code))
are indispensable parts of ((learning)) to program. Try to not just
glance over the examples—read them attentively and understand them.
This may be slow and confusing at first, but I promise that you'll
quickly get the hang of it. The same goes for the ((exercises)). Don't
assume you understand them until you've actually written a working
solution.

{{index interpretation}}

I recommend you try your solutions to exercises in an actual
JavaScript interpreter. That way, you'll get immediate feedback on
whether what you are doing is working, and, I hope, you'll be tempted
to ((experiment)) and go beyond the exercises.

{{if interactive

When reading this book in your browser, you can edit (and run) all
example programs by clicking them.

if}}

{{if book

{{index download, sandbox, "running code"}}

The easiest way to run the example code in the book, and to experiment
with it, is to look it up in the online version of the book at
[_https://eloquentjavascript.net_](https://eloquentjavascript.net/). There,
you can click any code example to edit and run it and to see the
output it produces. To work on the exercises, go to
[_https://eloquentjavascript.net/code_](https://eloquentjavascript.net/code),
which provides starting code for each coding exercise and allows you
to look at the solutions.

if}}

{{index "developer tools", "JavaScript console"}}

If you want to run the programs defined in this book outside of the
book's website, some care will be required. Many examples stand on their
own and should work in any JavaScript environment. But code in later
chapters is often written for a specific environment (the browser or
Node.js) and can run only there. In addition, many chapters define
bigger programs, and the pieces of code that appear in them depend on
each other or on external files. The
[sandbox](https://eloquentjavascript.net/code) on the website provides
links to Zip files containing all the scripts and data files
necessary to run the code for a given chapter.

## Overview of this book

This book contains roughly three parts. The first 12 chapters discuss
the JavaScript language. The next seven chapters are about web
((browsers)) and the way JavaScript is used to program them. Finally,
two chapters are devoted to ((Node.js)), another environment to
program JavaScript in.

Throughout the book, there are five _project chapters_, which describe
larger example programs to give you a taste of actual programming. In
order of appearance, we will work through building a [delivery
robot](robot), a [programming language](language), a [platform
game](game), a [pixel paint program](paint), and a [dynamic
website](skillsharing).

The language part of the book starts with four chapters that introduce
the basic structure of the JavaScript language. They introduce
[control structures](program_structure) (such as the `while` word you
saw in this introduction), [functions](functions) (writing your own
building blocks), and [data structures](data). After these, you will
be able to write basic programs. Next, Chapters [?](higher_order) and
[?](object) introduce techniques to use functions and objects to write
more _abstract_ code and keep complexity under control.

After a [first project chapter](robot), the language part of the book
continues with chapters on [error handling and bug fixing](error),
[regular expressions](regexp) (an important tool for working with
text), [modularity](modules) (another defense against complexity), and
[asynchronous programming](async) (dealing with events that take
time). The [second project chapter](language) concludes the first part
of the book.

The second part, Chapters [?](browser) to [?](paint), describes the
tools that browser JavaScript has access to. You'll learn to display
things on the screen (Chapters [?](dom) and [?](canvas)), respond to
user input ([Chapter ?](event)), and communicate over the network
([Chapter ?](http)). There are again two project chapters in this
part.

After that, [Chapter ?](node) describes Node.js, and [Chapter
?](skillsharing) builds a small website using that tool.

{{if commercial

Finally, [Chapter ?](fast) describes some of the considerations that
come up when optimizing JavaScript programs for speed.

if}}

## Typographic conventions

{{index "factorial function"}}

In this book, text written in a `monospaced` font will represent
elements of programs—sometimes they are self-sufficient fragments, and
sometimes they just refer to part of a nearby program. Programs (of
which you have already seen a few) are written as follows:

```
function factorial(n) {
  if (n == 0) {
    return 1;
  } else {
    return factorial(n - 1) * n;
  }
}
```

{{index "console.log"}}

Sometimes, to show the output that a program produces, the
expected output is written after it, with two slashes and an arrow in
front.

```
console.log(factorial(8));
// → 40320
```

Good luck!
