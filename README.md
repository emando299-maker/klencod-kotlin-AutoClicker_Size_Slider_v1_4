# Smart Auto Clicker — v1.1

مشروع Android Kotlin.

## الميزات
- أيقونة عائمة قابلة للتحريك تفتح وتغلق لوحة التحكم.
- لوحة كاملة وشريط مختصر.
- زر لإغلاق اللوحة والرجوع للأيقونة، وزر لإخفاء الأيقونة؛ يمكن إظهارها مجددًا من التطبيق.
- إضافة نقاط ضغط متعددة وحذف آخر نقطة.
- تحريك نقاط الضغط بالسحب.
- ضبط الفاصل من 0 إلى 86,400,000 مللي ثانية (يُنفّذ عمليًا بحد أدنى 1ms).
- رقم الإصدار 1.1 (versionCode 2) لتسهيل التحديث فوق النسخة السابقة عند استخدام نفس applicationId ومفتاح التوقيع.

## البناء
شغّل `./gradlew :app:assembleDebug`. يلزم استخدام نفس مفتاح توقيع النسخة المثبتة لتثبيت التحديث فوقها دون إزالة النسخة القديمة.


## Version 1.2 floating-window fix
The app now explicitly registers its in-app receiver as not exported on Android 13+, uses package-scoped broadcasts, and attempts to restore the floating bubble after returning from permission settings or reconnecting the accessibility service. Overlay permission and Accessibility Service still must be enabled by the user.
