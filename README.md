# روابط Gmube العميقة

صفحة واحدة تحوّل روابط الويب إلى مخطط التطبيق `gmube://`.

## الصيغ المدعومة

- `/gmube-links/watch/<videoId>` — يفتح درساً
- `/gmube-links/playlist/<playlistId>` — يفتح قائمة تشغيل
- `/gmube-links/?path=watch/<videoId>` — الصيغة القديمة، تبقى تعمل

## كيف تعمل بلا خادم

GitHub Pages يخدم `404.html` لأي مسار غير موجود، وهذا الملف نسخة حرفية من
`index.html`، فيقرأ المسار من `location.pathname` بدل معامل استعلام.

## App Links

عند توفّر التحقق (`.well-known/assetlinks.json` على جذر النطاق) يفتح أندرويد
الرابط في التطبيق مباشرة بلا صفحة وسيطة.
