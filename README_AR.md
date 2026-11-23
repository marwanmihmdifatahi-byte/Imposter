# MARO GAMES — Android project

تم وضع ملف اللعبة الأصلي كما هو داخل `www/index.html` وتجهيز إعدادات Capacitor الأساسية.

## مهم
هذا المشروع يحوّل اللعبة إلى تطبيق Android مستقل بأيقونة واسم خاصين، ويفتح بملء الشاشة بدون شريط المتصفح. واجهة اللعبة تعمل محليًا من ملفات التطبيق، ولا تحتاج اتصالًا بالإنترنت حسب الكود الحالي.
تقنيًا، Capacitor يعرض واجهة HTML/CSS/JavaScript داخل Android WebView؛ لذلك هذا ليس تطبيقًا Native بالكامل. التطبيق الـ Native بالكامل يتطلب إعادة بناء الواجهة والمنطق بتقنيات Android الأصلية.

## إنشاء APK (يتطلب كمبيوتر)
1. ثبّت Node.js و Android Studio.
2. فك ضغط المشروع.
3. افتح الطرفية داخل مجلد المشروع وشغّل:
   `npm install`
4. أضف منصة Android:
   `npx cap add android`
5. انسخ ملفات اللعبة إلى مشروع Android:
   `npx cap sync android`
6. افتح Android Studio:
   `npx cap open android`
7. من Android Studio اختر Build > Build Bundle(s) / APK(s) > Build APK(s).

## ملاحظات
- لم يتم إنشاء APK داخل هذه الحزمة؛ يلزم Android SDK/Gradle لبنائه.
- لم يتم تعديل كود اللعبة الأصلي.
- اسم التطبيق: MARO GAMES
- معرّف التطبيق: com.marogames.pro
