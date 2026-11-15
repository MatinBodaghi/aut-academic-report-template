# قالب مدرن گزارش، مقاله و پروژه‌های آکادمیک دانشگاه صنعتی امیرکبیر
# Modern AUT Academic Report, Paper & Project LaTeX Template

[![LaTeX XeTeX](https://img.shields.io/badge/LaTeX-XeTeX-blue.svg?logo=latex)](https://www.latex-project.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Compile LaTeX Document](https://img.shields.io/badge/CI-GitHub%20Actions-blue?logo=githubactions)](../../actions)
[![Template](https://img.shields.io/badge/GitHub-Template-brightgreen.svg)](#نحوه-استفاده-از-این-مخزن-به-عنوان-template)

قالب جامع، ماژولار و استاندارد برای نگارش **گزارش‌های کار آزمایشگاهی، پروژه‌های پایانی دروس، سمینارها و مقالات پژوهشی** به زبان فارسی و انگلیسی بر پایه موتور `XeLaTeX` و بسته قدرتمند `XePersian`، به همراه استایل رسمی دانشگاه صنعتی امیرکبیر (پلی‌تکنیک تهران).

---

## 🌟 ویژگی‌های برجسته (Key Features)

- **سربرگ پارامتریک و مدرن (Dynamic Academic Header):**
  - دارای لوگوی رسمی دانشگاه صنعتی امیرکبیر و دانشکده مهندسی برق.
  - پشتیبانی از نگارش **تک‌نفره** (نام، شماره دانشجویی، ایمیل) یا **گروهی** (سوئیچ خودکار کادر مشخصات).
  - متغیرهای تعریف‌شده در ابتدای سند (`\reportTitle`، `\courseName`، `\instructorName`، `\semester` و ...).

- **طراحی ماژولار استایل (`report-style.sty`):**
  - جداسازی کامل تنظیمات صفحه، بسته‌ها، فونت‌ها و رنگ‌ها از متن اصلی.
  - تنظیم حاشیه‌های دقیق و بهینه مهندسی با بسته `geometry`.
  - سرصفحه و پاصفحه مدرن با خط جداکننده باریک و شماره صفحه فارسی (`fancyhdr`).

- **کادرهای رنگی پیشرفته (`tcolorbox`):**
  - کادر نکته (`noteBox`)، کادر قضایا و فرمول‌های کلیدی (`theoremBox`) و کادر هشدار و نکات مهم (`warningBox`).

- **رسم برداری مدارها، نمودارها و فلوچارت‌ها (Vector Graphics & Flowcharts):**
  - رسم انواع شماتیک‌های مداری الکتریکی با بسته `circuitikz` (استاندارد IEEE / American).
  - ترسیم مستقیم نمودارهای ریاضیاتی و توابع دوبعدی با بسته `pgfplots`.
  - رسم فلوچارت‌های استاندارد الگوریتمی و فرآیندی با گره‌های آماده `TikZ` (`flowStartEnd`، `flowProcess`، `flowDecision`، `flowIO`، `flowArrow`).

- **محیط کدنویسی استاندارد (`listings`):**
  - تنظیم استایل `modernCode` با شماره خطوط، تفکیک رنگی سینتکس و کادر اختصاصی.
  - سازگار کامل با موتور دوزبانه و بدون خطای Bidi.

- **جدول‌های مهندسی شکیل (`booktabs` و `tabularx`):**
  - جداول سه خطی استاندارد مجلات و مقالات معتبر بدون خطوط عمودی زشت.

- **مدیریت مراجع (`BibTeX`):**
  - فایل `references.bib` استاندارد با استایل `ieeetr`.

- **اتوماسیون ابری (GitHub Actions CI/CD):**
  - دارای گردش‌کار `.github/workflows/compile.yml` که به ازای هر `push`، گزارش را روی سرور اوبونتو با `xelatex` کامپایل کرده و فایل خروجی `main.pdf` را برای دانلود آماده می‌کند.

- **پیکربندی حرفه‌ای VS Code:**
  - دارای `.vscode/settings.json` با دستورهای آماده کامپایل تک‌کلیکه با اکستنشن `LaTeX Workshop`.

- **همراه‌سازی فونت‌ها در مخزن:**
  - فونت‌های آزاد و استاندارد فارسی (`BNazanin` و `BTitr`) داخل پوشه `fonts/` قرار داده شده‌اند تا روی لینوکس، مک و سرور گیت‌هاب بدون نیاز به نصب دستی کامپایل شوند.

---

## 📂 ساختار فایل‌های مخزن (Project Structure)

```text
aut-academic-report-template/
├── .github/
│   └── workflows/
│       └── compile.yml        # کامپایل ابری خودکار با گیت‌هاب اکشنز
├── .vscode/
│   └── settings.json          # تنظیمات کامپایل سریع در VS Code
├── fonts/                     # فونت‌های فارسی موردنیاز (B Nazanin, B Titr)
│   ├── BNazanin.ttf
│   └── BTitrBd.ttf
├── figures/                   # دیاگرام‌ها و نمودارهای برداری
├── images/                    # اسکرین‌شات‌ها و تصاویر گزارش
├── logos/                     # لوگوی دانشگاه و دانشکده
│   ├── aut-logo.png
│   └── EE-aut.jpg
├── .gitignore                 # نادیده گرفتن فایل‌های موقت لاتک
├── LICENSE                    # مجوز MIT
├── README.md                  # راهنمای جامع مخزن
├── main.tex                   # سند اصلی و دمو جامع قالب
├── report-style.sty           # پکیج استایل، کادرها و ماکروها
└── references.bib             # فایل دیتابیس مراجع BibTeX
```

---

## 🚀 راهنمای سریع راه‌اندازی (Quick Start)

### ۱. پیش‌نیازها
- توزیع لاتک: **TeX Live 2022 یا جدیدتر** (یا MiKTeX به‌روز).
- موتور کامپایل: **XeLaTeX** (به دلیل استفاده از زبان فارسی و بسته `xepersian`).

### ۲. کامپایل با خط فرمان (Terminal / CMD / PowerShell)
در پوشه پروژه دستورهای زیر را اجرا کنید:

```bash
xelatex main.tex
bibtex main
xelatex main.tex
xelatex main.tex
```

### ۳. کامپایل در VS Code
1. اکستنشن [LaTeX Workshop](https://marketplace.visualstudio.com/items?itemName=James-Yu.latex-workshop) را نصب کنید.
2. با فشردن کلیدهای `Ctrl + Alt + B` سند شما به طور خودکار طبق تنظیمات `.vscode/settings.json` با چرخه کامل `XeLaTeX ➔ BibTeX ➔ XeLaTeX ➔ XeLaTeX` کامپایل خواهد شد.
3. با کلیدهای `Ctrl + Alt + V` پیش‌نمایش زنده PDF را مشاهده کنید.

---

## ⚙️ شخصی‌سازی مشخصات گزارش (Customization)

در ابتدای فایل `main.tex`، متغیرهای گزارش به سادگی قابل ویرایش هستند:

```latex
% مشخصات اصلی گزارش / پروژه
\newcommand{\ReportTitle}{عنوان پروژه یا گزارش کار}
\newcommand{\ReportSubtitle}{زیرعنوان گزارش یا پروژه}
\newcommand{\CourseName}{نام درس}
\newcommand{\ProfessorName}{استاد درس: نام استاد}
\newcommand{\Semester}{نیم‌سال تحصیلی}

% مشخصات نویسنده (حالت تک‌نفره)
\newcommand{\AuthorName}{نام و نام خانوادگی}
\newcommand{\StudentNumber}{۱۲۳۴۵۶۷۸}
\newcommand{\StudentEmail}{student@aut.ac.ir}
```

> **نکته:** برای گزارش‌های گروهی، کافی است کادر جدول مشخصات را در بدنه `main.tex` بر اساس کامنت‌های راهنما فعال کنید.

---

## 🎨 نمونه‌های کاربردی (Usage Cheatsheet)

### ۱. کادرهای رنگی (`tcolorbox`)
```latex
\begin{noteBox}[عنوان نکته]
متن توضیحات نکته موردنظر...
\end{noteBox}

\begin{theoremBox}[قضیه تونن]
هر مدار خطی دوپایانه را می‌توان با یک منبع ولتاژ و مقاومت سری معادل کرد.
\end{theoremBox}

\begin{warningBox}[احتیاط]
پیش از اتصال منبع، از صفر بودن ولتاژ اطمینان حاصل فرمایید.
\end{warningBox}
```

### ۲. رسم مدار با `circuitikz`
```latex
\begin{circuitikz}[american]
    \draw (0,0) to[sV, l=$V_{\mathrm{in}}$] (0,3)
          -- (1,3) to[R, l=$R$] (3,3)
          -- (4,3) to[C, l=$C$] (4,0)
          -- (0,0);
\end{circuitikz}
```

### ۳. رسم فلوچارت با `TikZ`
```latex
\begin{tikzpicture}[node distance=1.2cm and 2cm]
    \node (start) [flowStartEnd] {\rl{شروع}};
    \node (proc)  [flowProcess, below=of start] {\rl{محاسبات مداری}};
    \node (stop)  [flowStartEnd, below=of proc] {\rl{پایان}};
    \draw [flowArrow] (start) -- (proc);
    \draw [flowArrow] (proc) -- (stop);
\end{tikzpicture}
```

### ۴. درج کد برنامه‌نویسی
```latex
\begin{latin}
\begin{lstlisting}[language=Python, caption={Resonance Calculation}]
def calc_f0(L, C):
    return 1.0 / (2 * 3.14159 * (L * C)**0.5)
\end{lstlisting}
\end{latin}
```

---

## 📦 نحوه استفاده از این مخزن به عنوان Template در گیت‌هاب

1. در بالای صفحه ریپازیتوری در گیت‌هاب، روی دکمه سبز رنگ **Use this template** کلیک کنید.
2. گزینه **Create a new repository** را انتخاب کنید.
3. یک ریپازیتوری جدید برای پروژه یا گزارش کار خود ایجاد نمایید و شروع به نوشتن کنید!
4. به محض اولین `git push`، گیت‌هاب اکشنز به صورت رایگان فایل PDF گزارش شما را کامپایل کرده و در بخش **Actions > Artifacts** در اختیارتان می‌گذارد.

---

## 📄 مجوز (License)

این پروژه تحت مجوز [MIT](LICENSE) منتشر شده است و استفاده از آن برای کلیه دانشجویان، پژوهشگران و اساتید با حفظ کپی‌رایت آزاد است.

---
**دانشگاه صنعتی امیرکبیر (پلی‌تکنیک تهران)**  
*دانشکده مهندسی برق و کامپیوتر*
