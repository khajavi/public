<div dir="rtl">
در این صفحه سعی می کنم چکیده‌ای از دانشی که به مرور زمان در مورد فرآیند تولید نرم‌افزار کسب می‌کنم را مکتوب کنم.

# فرآیند توسعه نرم‌افزار (Software Development Process)
در [این صفحه](http://www.selectbs.com/analysis-and-design/what-is-a-software-development-process) روند تولید نرم‌افزار به به مراحل زیر تقسیم کرده است:
<div dir="ltr">
* Requirements Analysis
* Specification
* Software architecture
* Implementation
* Testing
* Documentation
* Training and Support
* Maintenance
<div dir="rtl">

در [این صفحهٔ ویکی‌پدیا](http://en.wikipedia.org/wiki/Software_development_process) نیز فرآیند تولید نرم‌افزار به سه مرحلهٔ مهم تقسیم شده است:
<div dir="ltr">
* Planning
* Implementation, testing and documenting
* Deployment and maintenance
<div dir="rtl">

# تحلیل نیازمندی‌ها (Requirements Analysis)
در مدل آبشاری تحلیل نیازمندی‌ها در فاز اول تنظیم شده است اما در متدهای توسعهٔ نرم‌افزار اخیر در تمام دورهٔ حیات تولید نرم‌افزار، تحلیل نیازمندی وجود دارد، از جمله در متدهای RUP و Extreme Programming و اسکرام. [بیشتر](http://en.wikipedia.org/wiki/Requirements_engineering)

# Functional Requirements
نیازمندی‌هایی که سیستم باید `انجام دهد`. مثلاً

<div dir="ltr">
```
System shall do <...>
```
<div dir="rtl">
* سیستم باید بتواند هویت کاربر را تشخیص دهد.
* کاربر سیستم باید بتواند گذرواژهٔ خود را تغییر دهد.

بیشتر:

* http://c2.com/cgi/wiki?FunctionalRequirements

# Non-functional requirements
نیازمندی‌هایی که سیستم باید آن طور `باشد`‍. به این نیازمندی‌های ایلیتیز (ilities) هم می‌گویند به این خاطر که معمولاً به صورت زیر عنوان می‌شود.
<div dir="ltr">
* usability
* reliability
* interoperability
* scalability
* security
<div dir="rtl">
- [فهرست کامل نیازمندی‌های غیرتابعی](list-of-nunfunctional-requirement.md)

چند مثال

<div dir="ltr">
```
System shall be <...>
```
<div dir="rtl">
* سیستم باید چند-سکویی باشد و روی سیستم‌عامل‌های مختلف اجرا شود.
* سیستم باید تحت وب باشد.

بیشتر:
* http://c2.com/cgi/wiki?NonFunctionalRequirements
* http://en.wikipedia.org/wiki/Non-functional_requirement


# مراحل
تحلیل نیازمندی‌ها به [سه قسمت](http://en.wikipedia.org/wiki/Requirements_analysis) تقسیم می‌شود:

* استخراج نیازمندی‌ها
* تحلیل نیازمندی‌ها
* ثبت و مستندسازی نیازمندی‌ها

### استخراج نیازمندی‌ها(جمع آوری)

روش‌ها
<div dir="ltr">
* interviews
* questionnaires
* user observation
* workshops
* brain storming
* use cases
* role playing
* prototyping
<div dir="rtl">
مشکلات
<div dir="ltr">
* Problems of scope
* Problems of understanding
* Problems of volatility
<div dir="rtl">

### تحلیل نیازمندی‌ها

### ثبت و مستندسازی نیازمندی‌ها

به دو روش می‌توانیم نیازمندی‌ها را مستند کنیم.

#### Use Case

یوز کیس در نمودارهای UML تعریف شده است اما این نمودارها ارزش کمی دارند در صورتی که ارزش کلیدی یوزکیس‌ها آن متونی‌ست که در UML استاندارد نشده است. بنابراین انرژی‌تان را روی متن‌ها بگذارید. به نظر مارتین فالر، بهترین کتاب برای آشنایی با یوزکیس‌ها، کتاب Writing Effective Use Cases نوشتهٔ Alistair Cockburn است.

یک سناریوی واقعی.

از روی Use Case باید بتوانیم Acceptance Test بنویسیم.

اطلاعات بیشتر:
* http://martinfowler.com/bliki/UseCase.html

#### User Story
مفهوم داستان کاربری از XP گرفته شده و معمولاً در روش‌های چابک از آن استفاده می‌شود.

مارتین فالر، ۵ مشخصه برای داستان‌های کاربری خوب [معرفی می‌کند](http://martinfowler.com/bliki/UserStory.html):
<div dir="ltr">
* Independent
* Negotiable
* Valuable
* Estimable
* Small
* Testable
<div dir="rtl">
فرم نوشتن داستان‌کاربری به صورت زیر است:
<div dir="ltr">
```
"As a … I want … So that …"
```
<div dir="rtl">


معرفی کتاب برای نوشتن داستان کاربری:

* User Stories Applied: For Agile Software Development by Mike Cohn

#### فرق بین داستان کاربری و یوزکیس
داستان‌های کاربری در متد XP نیازمندی‌ها را به قطعات کوچکی جهت برنامه‌ریزی (مثلاً برنامه‌ریزی برای اسپرینت) تقسیم می‌کند.

یوزکیس‌ها نیازمندی‌ها را از دیدگاه کاربران، سازماندهی می‌کنند. آن‌ها بر روی اهداف کاربران، و چگونگی تعامل کاربران با سیستم تمرکز می‌کنند.

اطلاعات بیشتر: http://martinfowler.com/bliki/UseCasesAndStories.html

# معرفی کتاب

کتاب Applying UML and Patterns: An Introduction to Object-Oriented Analysis and Design and Iterative Development, Third Edition By Craig Larman را بررسی کردم. کتاب بسیار مفیدی به نظر می‌رسد که به نظرم باید در وهلهٔ اول این کتاب را بخوانیم. فهرست مطالب این کتاب را در [این نشانی](Applying UML and Patterns: An Introduction to Object-Oriented Analysis and Design and Iterative Development, Third Edition By Craig Larman) قرار داده‌ام.

# اطلاعات بیشتر

* https://sites.google.com/site/yacoset/Home/how-to-design-a-computer-program

# تبادل نظر

[gimmick:Disqus](senotes)
