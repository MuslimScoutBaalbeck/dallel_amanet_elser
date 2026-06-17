# دليل أمانة السر الكشفية — مشروع Quarto كامل

هذا المجلد يحتوي نسخة Quarto كاملة من دليل أمانة السر الكشفية، مهيأة للنشر كـ HTML Book على GitHub Pages.

## التشغيل المحلي

```bash
quarto preview
```

## توليد HTML

```bash
quarto render --to html
```

سيتم توليد الموقع داخل مجلد `docs/` لأن GitHub Pages مضبوط عادة على `main / docs`.

## النشر على GitHub Pages

1. ارفع المشروع إلى المستودع.
2. نفّذ محليًا:

```bash
quarto render --to html
git add .
git commit -m "Render Quarto HTML book"
git push
```

3. في GitHub Pages اختر: `Deploy from a branch` ثم `main` ثم `/docs`.

## ملاحظات

- تم التركيز على HTML لأنه أنسب للعربية والـRTL من PDF عبر LaTeX.
- ملف Word الأصلي موجود للرجوع إليه: `source_dalil_amanat_al_sirr.docx`.
- الصور الأساسية موجودة في `assets/images/`.
- يمكن تعديل التصميم من `styles/book-design.css`.
