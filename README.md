# TokenForge

**A lightweight toolkit for improving AI workflow efficiency, reducing unnecessary token usage, and encouraging better verification practices.**

[English](#english) · [فارسی](#فارسی) · **[Main Prompt →](./PROMPT.md)**

> **Want to use TokenForge with Claude?**
> **[Open the Main Prompt →](./PROMPT.md)**

---

# English

## What is TokenForge?

**TokenForge** is a collection of practical prompts and tools designed to help users work more efficiently with AI assistants such as Claude.

Its main goals are:

* Reduce unnecessary token usage.
* Improve response efficiency.
* Preserve important requirements and context.
* Encourage AI to verify generated code and files before delivery.
* Reduce repetitive and unnecessary output.
* Improve the reliability of AI-assisted development.

TokenForge is designed to be useful for **everyone**, from beginners to developers and advanced AI users.

## Main Prompt

The main public prompt is available here:

### **[→ Open PROMPT.md](./PROMPT.md)**

You can copy the prompt and paste it into Claude to enable the workflow.

The prompt encourages Claude to:

**Understand → Build → Test → Fix → Retest → Verify → Deliver**

It specifically instructs Claude not to claim that code or files work unless they have actually been verified.

## What Does It Help With?

TokenForge can be useful when working with:

* Python
* JavaScript
* HTML/CSS
* Websites
* Windows applications
* Scripts
* APIs
* Configuration files
* Automation
* Software projects
* Generated files
* AI-assisted coding

## Verification Philosophy

One of the main principles of TokenForge is:

> **Writing something is not the same as verifying it.**

AI-generated code can look correct while still containing syntax errors, missing dependencies, broken logic, or configuration problems.

TokenForge encourages a workflow where the AI:

1. Understands the task.
2. Creates or modifies the result.
3. Tests what can actually be tested.
4. Finds problems.
5. Fixes them.
6. Tests again.
7. Reports what was actually verified.

## Test Statuses

When appropriate, the system uses clear verification states:

| Status         | Meaning                                                |
| -------------- | ------------------------------------------------------ |
| **PASS**       | Successfully tested                                    |
| **FAIL**       | Tested and failed                                      |
| **FIXED**      | Failed initially, then fixed and successfully retested |
| **BLOCKED**    | Testing was prevented by an environment limitation     |
| **NOT TESTED** | Could not reasonably be tested                         |

This helps prevent unverified results from being presented as guaranteed working.

## Token Efficiency

Token efficiency does **not** mean making every response extremely short.

The goal is:

> **Maximum useful information per token.**

TokenForge encourages AI to remove:

* Repetition
* Filler
* Unnecessary explanations
* Duplicate code
* Unnecessary alternatives

while preserving:

* Requirements
* Important context
* Technical details
* Error handling
* Edge cases
* Safety requirements
* Required output formats

## Who Can Use It?

Anyone can use TokenForge.

You do not need to be a programmer.

It can be useful for:

* Students
* Developers
* AI users
* Researchers
* Content creators
* Software engineers
* People building projects with Claude

## Quick Start

### 1. Open the prompt

**[Open PROMPT.md →](./PROMPT.md)**

### 2. Copy the prompt

Copy the complete prompt from `PROMPT.md`.

### 3. Paste it into Claude

Start a Claude conversation and provide the prompt.

### 4. Give Claude your task

Then provide your normal request, such as:

> Build this application.

or:

> Fix this project.

Claude should then follow the verification workflow before presenting the final result.

## Important Limitation

The prompt cannot give an AI capabilities that its environment does not provide.

For example, if Claude cannot access:

* A required API
* Specific hardware
* A private server
* Missing software
* Required credentials
* An unavailable dependency

it cannot genuinely test those components.

The correct behavior is to report the limitation instead of pretending the test succeeded.

## Repository Structure

```text
tokenforge/
├── README.md
├── PROMPT.md
├── .gitignore
├── src/
├── tests/
├── examples/
└── results/
```

## Principle

**Build it. Test it. Fix it. Test it again. Then deliver it.**

---

# فارسی

## TokenForge چیست؟

**TokenForge** مجموعه‌ای از پرامپت‌ها و ابزارهای کاربردی برای کار بهتر و بهینه‌تر با دستیارهای هوش مصنوعی مانند Claude است.

هدف‌های اصلی آن:

* کاهش مصرف غیرضروری توکن
* افزایش بهره‌وری پاسخ‌ها
* حفظ نیازمندی‌ها و اطلاعات مهم
* تشویق هوش مصنوعی به تست کد و فایل قبل از تحویل
* کاهش خروجی‌های تکراری و غیرضروری
* افزایش قابلیت اطمینان در توسعه با کمک هوش مصنوعی

TokenForge برای **همه کاربران** طراحی شده است؛ از کاربران مبتدی تا برنامه‌نویسان و کاربران حرفه‌ای هوش مصنوعی.

## پرامپت اصلی

پرامپت اصلی پروژه از اینجا در دسترس است:

### **[→ باز کردن PROMPT.md](./PROMPT.md)**

می‌توانید آن را کپی کرده و داخل Claude قرار دهید.

این پرامپت Claude را تشویق می‌کند که روند زیر را دنبال کند:

**درک → ساخت → تست → رفع مشکل → تست مجدد → بررسی → تحویل**

همچنین به Claude تأکید می‌کند که نباید ادعا کند یک کد یا فایل کار می‌کند، مگر اینکه واقعاً امکان بررسی و تست آن وجود داشته باشد.

## برای چه کارهایی مناسب است؟

TokenForge می‌تواند برای موارد زیر استفاده شود:

* Python
* JavaScript
* HTML/CSS
* وب‌سایت‌ها
* برنامه‌های Windows
* اسکریپت‌ها
* APIها
* فایل‌های تنظیمات
* Automation
* پروژه‌های نرم‌افزاری
* فایل‌های تولیدشده توسط AI
* برنامه‌نویسی با کمک هوش مصنوعی

## فلسفه تست و بررسی

یکی از اصول اصلی TokenForge این است:

> **نوشتن یک چیز با بررسی کردن آن یکسان نیست.**

ممکن است کدی که توسط AI تولید شده در ظاهر درست باشد، اما دارای خطای Syntax، وابستگی ناقص، مشکل منطقی یا تنظیمات اشتباه باشد.

TokenForge یک روند مشخص را پیشنهاد می‌کند:

1. درک درخواست
2. ساخت یا تغییر نتیجه
3. تست مواردی که واقعاً امکان تست دارند
4. پیدا کردن مشکلات
5. رفع مشکلات
6. تست مجدد
7. گزارش نتیجه واقعی تست

## وضعیت‌های تست

در صورت نیاز از وضعیت‌های مشخص استفاده می‌شود:

| وضعیت          | معنی                                 |
| -------------- | ------------------------------------ |
| **PASS**       | با موفقیت تست شده                    |
| **FAIL**       | تست شده و شکست خورده                 |
| **FIXED**      | مشکل پیدا و رفع شده و دوباره تست شده |
| **BLOCKED**    | به دلیل محدودیت محیط قابل تست نبوده  |
| **NOT TESTED** | امکان تست منطقی آن وجود نداشته       |

این کار کمک می‌کند نتایج تست‌نشده به‌عنوان نتیجه قطعی معرفی نشوند.

## بهینه‌سازی مصرف توکن

بهینه‌سازی توکن به معنی کوتاه کردن اجباری همه پاسخ‌ها نیست.

هدف این است:

> **بیشترین اطلاعات مفید با کمترین توکن غیرضروری.**

TokenForge مواردی مانند:

* تکرار
* جملات اضافی
* توضیحات غیرضروری
* کد تکراری
* راه‌حل‌های اضافی

را تا حد امکان کاهش می‌دهد؛ اما موارد مهم مانند:

* نیازمندی‌ها
* اطلاعات مهم
* جزئیات فنی
* مدیریت خطا
* Edge Caseها
* الزامات ایمنی
* فرمت خروجی

نباید حذف شوند.

## چه کسانی می‌توانند استفاده کنند؟

همه می‌توانند از TokenForge استفاده کنند.

نیازی به برنامه‌نویس بودن نیست.

مناسب برای:

* دانش‌آموزان
* برنامه‌نویسان
* کاربران AI
* پژوهشگران
* تولیدکنندگان محتوا
* مهندسان نرم‌افزار
* افرادی که با Claude پروژه می‌سازند

## شروع سریع

### ۱. پرامپت را باز کنید

**[باز کردن PROMPT.md →](./PROMPT.md)**

### ۲. پرامپت را کپی کنید

کل محتوای `PROMPT.md` را کپی کنید.

### ۳. آن را داخل Claude قرار دهید

یک گفت‌وگو در Claude ایجاد کرده و پرامپت را وارد کنید.

### ۴. درخواست خود را بدهید

سپس درخواست معمول خود را بنویسید؛ مثلاً:

> این برنامه را بساز.

یا:

> این پروژه را اصلاح کن.

Claude باید قبل از ارائه نتیجه نهایی، تا جایی که محیط اجازه می‌دهد آن را بررسی و تست کند.

## محدودیت مهم

این پرامپت نمی‌تواند قابلیت‌هایی را که محیط Claude در اختیار ندارد ایجاد کند.

برای مثال، اگر Claude به موارد زیر دسترسی نداشته باشد:

* API موردنیاز
* سخت‌افزار خاص
* سرور خصوصی
* نرم‌افزار موردنیاز
* اطلاعات ورود
* Dependency موجود نبودن

نمی‌تواند آن بخش را واقعاً تست کند.

در چنین شرایطی باید محدودیت را اعلام کند و **نباید وانمود کند که تست با موفقیت انجام شده است.**

## ساختار پروژه

```text
tokenforge/
├── README.md
├── PROMPT.md
├── .gitignore
├── src/
├── tests/
├── examples/
└── results/
```

## اصل اصلی

**بساز. تست کن. مشکل را رفع کن. دوباره تست کن. سپس تحویل بده.**

---

## License

This project intentionally does not include a license file.
