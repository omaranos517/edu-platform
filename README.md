# المنصة التعليمية (قيد التطوير حالياً)

منصة تعليمية مبنية باستخدام Laravel تهدف إلى تقديم محتوى تعليمي مميز للطلاب في مختلف المراحل الدراسية.

![Laravel Logo](https://laravel.com/img/logomark.min.svg)

## 🚀 المميزات

- نظام تسجيل دخول وتسجيل مستخدمين
- إدارة المحتوى التعليمي (دروس، ملفات، فيديوهات)
- واجهة مستخدم بسيطة وسهلة الاستخدام
- تكامل مع قواعد البيانات ورفع الملفات

## 📦 التقنيات المستخدمة

### Backend

- Laravel 12
- PHP 8.x
- MySQL

### Frontend

الان

- Blade Templates ( stracks, layouts, views, components )
- Vite
  قريباً
- Vue.js
- Inertia.js

## ⚙️ متطلبات التثبيت

- Git
- Docker
- Docker Compose

## 🔁 التطويرات المستقبلية

### المميزات التقنية

- استخدام اطار عمل للواجهة (Vue.js)

### تجربة المستخدم

- عمل نظام ادارة للمنصة يكون عن طريق هيكل الإدارة التالي :
    - مسؤول عن المنصة ومعلمين وكل معلم له مواد يستطيع الوصول لها والتحكم بمحتواها
- تحويل الموقع ليكون SPA عن طريق استخدام اطار عمل للواجهة

## 🛠 التثبيت

```bash
git clone https://github.com/omaranos517/edu-platform.git
cd edu-platform
cp .env.example .env
docker run --rm \
-v $(pwd):/app \
-w /app \
composer install
./vendor/bin/sail up -d
./vendor/bin/sail composer install
./vendor/bin/sail artisan key:generate
./vendor/bin/sail npm install
./vendor/bin/sail artisan migrate --seed
```

## بدأ المشروع

```bash
# 1. شغل الحاويات في الخلفية
./vendor/bin/sail up -d
```

إذا كنت تريد تشغيل Vite فقط بدون الـ queue والخادم الرئيسي، استخدم:

```bash
./vendor/bin/sail npm run dev
```

## 🔐 الترخيص

هذا المشروع مرخّص تحت رخصة MIT.  
راجع ملف [LICENSE](LICENSE).
