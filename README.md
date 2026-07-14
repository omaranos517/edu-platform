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

- PHP ≥ 8.1
- Composer
- Node.js + npm
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
git clone https://github.com/omaranos517/myPlatform.git
cd edu-platform
cp .env.example .env
docker compose up -d
composer install
php artisan key:generate
npm install
php artisan migrate
php artisan db:seed
composer run dev
```

## 🔐 الترخيص

هذا المشروع مرخّص تحت رخصة MIT.  
راجع ملف [LICENSE](LICENSE).
