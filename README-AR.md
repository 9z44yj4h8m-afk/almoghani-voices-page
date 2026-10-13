# صفحة الأصوات — ALMOGHANI LIVE

## ملف البداية (index)
- `src/routes/admin-voices.tsx` — صفحة لوحة الأصوات على العنوان `/admin-voices`.
- `src/routes/100.tsx` — صفحة لوحة الخصائص على العنوان `/100` (إضافة/حذف صوت، النصوص، الألوان).

## بقية الملفات
| الملف | الوظيفة |
|---|---|
| `src/components/admin/voice-chat-manager.tsx` | واجهة اللوحة: النص، اختيار الصوت، الغناء، تجربة الصوت، الحفظ |
| `src/lib/voice-config.ts` | قائمة أصوات البَنات وتقسيمها والألحان والإيقاعات |
| `src/lib/voice-panel.ts` | نصوص وألوان اللوحة وحالة الإخفاء والأصوات المضافة |
| `src/lib/voice-preview.functions.ts` | تشغيل الصوت من الخادم (تجربة الصوت) |
| `src/routes/api/public/voice-listen.ts` | تحويل كلامك المسجّل إلى نص |
| `src/components/admin/password-login.tsx` | دخول لوحة التحكم بكلمة المرور |
| `src/components/member-provider.tsx` | حالة العضو/المالك |
| `src/components/ui/{button,switch,dialog}.tsx` | أزرار ومفاتيح ونافذة الإعدادات |
| `src/styles.css` | كل التنسيقات، وأقسام `voice-studio` و `voice-neon` تخص هذه الصفحة |
| `src/assets/voice-anime-header-v2.jpg` + `.asset.json` | صورة الشعار أعلى اللوحة |
| `src/assets/voice-anime-avatar-v2.jpg` + `.asset.json` | صورة الأفاتار الدائرية |
| `public/admin-voices.webmanifest` | ملف التثبيت كـتطبيق على آيفون |

## التشغيل
```
bun install
bun run dev
```
تحتاج ملف `.env` (غير مضمّن هنا) بقيم: `VITE_SUPABASE_URL`، `VITE_SUPABASE_PUBLISHABLE_KEY`، و`LOVABLE_API_KEY` لتجربة الصوت.

## ملاحظة
هذه الملفات جزء من مشروع واحد؛ لفتحها عندك انسخها فوق نفس المسارات في المشروع الكامل، أو استخدم أرشيف `almoghani-live-source.zip`.
