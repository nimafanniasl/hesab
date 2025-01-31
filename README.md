حساب
---

یک نرم‌افزار خط‌فرمان حسابداری شخصی با تقویم شمسی

# نصب و استفاده

با دستور زیر حساب را نصب کنید. پس از اجرا به دستور `hesab` در خط‌فرمان دسترسی خواهید داشت.
```bash
$ curl "https://raw.githubusercontent.com/ekm507/hesab/main/install.sh" | bash
```

# برای توسعه

نرم‌افزار هنوز شدیداً در حال توسعه است اما می‌توانید چنین استفاده‌اش کنید:
1. اول مخزن رو بارگیری کنید.
2. یک محیط مجازی پایتون بسازید.
3. نیازمندی‌ها رو نصب کنید.
4. اسکریپت رو اجرا کنید.

دستورهای زیر برای مرحله‌های ۱ تا ۳:
```bash
git clone "https://github.com/ekm507/hesab"
cd hesab
python3 -m venv .venv
source .venv/bin/activate
python -m pip install -r requirements.txt
```

اجرا با چند مثال:
```bash
./hesab --help
./hesab add "ice cream" -20
./hesab list
```

تصویر نمونه
![image](https://github.com/ekm507/hesab/assets/13185969/4669047b-8c06-4166-bcaa-bf03192fbea0)


# نقشهٔ راه توسعه
در هر نگارش اصلی قرار است یک سری ویژگی به نرم‌افزار افزوده شوند.

#### نگارش ۰٫۱
ویژگی‌هایی که انتظار می‌رود در اولین انتشار این نرم‌افزار موجود باشند:
- یک ابزار پایدار با رابط خط‌فرمان قابل‌استفاده
- امکان ذخیره و نمایش دخل‌وخرج‌ها

#### نگارش ۱
ویژگی‌هایی که انتظار می‌رود در نگارش ۱ نرم‌افزار موجود باشند:
- یک رابط خط‌فرمان قابل‌استفاده، ساده و زیبا
- امکان ذخیره کردن عنوان هزینه‌ها و در‌آمدها، مقدار پول و تاریخ آن‌ها به همراه اطلاعات اضافی شامل توضیحات و قیمت بر حسب یکای جایگزین
- یک بسته‌بندی مناسب و قابل‌نصب برای نرم‌افزار
