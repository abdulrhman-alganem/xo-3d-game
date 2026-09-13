# XO 3D Android

نسخة Android من لعبة XO 3D للموبايل.

- تعمل بالكامل بدون إنترنت.
- واجهة مخصصة للموبايل.
- لعب ضد الكمبيوتر أو شخصين.
- مستويات سهل / متوسط / صعب.
- أصوات ومؤثرات فوز.
- تستهدف Android 16 / API 36 بما يتوافق مع متطلبات Google Play الحالية للتطبيقات الجديدة.
- GitHub Actions يبني APK للتجربة وAAB للنشر.

## Build

الـ workflow يثبت JDK 17 وGradle 9.6 وAndroid SDK 36 على GitHub Actions ثم يبني التطبيق.

## توقيع Google Play

الـ APK التجريبي يبنى مباشرة. الـ AAB يكون موقّعًا فقط عند إضافة أسرار التوقيع إلى GitHub Actions:

- ANDROID_KEYSTORE_BASE64
- KEYSTORE_PASSWORD
- KEY_ALIAS
- KEY_PASSWORD

لا تضع ملف keystore أو كلمات المرور داخل المستودع العام.
