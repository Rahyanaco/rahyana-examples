[FA] فارسی | [EN](./README.en.md)

<div dir="rtl">

# هاب مثال‌های [راهیانا](https://rahyana.ir) ✨

به مرکز رسمی مثال‌ها و پروژه‌های آموزشی راهیانا خوش آمدید. این ریپو «هاب» تمام مثال‌های زبان‌های مختلف را یک‌جا معرفی و لینک می‌کند تا سریع‌تر شروع کنید و بهترین مسیر را پیدا کنید.

## 🚀 شروع سریع
- نشانی تولید <span dir="ltr">API</span>: <code><span dir="ltr">https://rahyana.ir/api/v1</span></code>
- برای تست محلی: متغیرهای محیطی `API_KEY_OVERRIDE` و `BASE_URL_OVERRIDE`
- مدل‌های محبوب: `openai/gpt-5` ، `openai/gpt-4o`

## 📎 مرور سریع نکات مشترک API
- **آدرس پایه**: <code><span dir="ltr">https://rahyana.ir/api/v1</span></code>
- **احراز هویت**: هدر <code><span dir="ltr">Authorization: Bearer YOUR_API_KEY</span></code>
- **مدل‌ها**: دریافت فهرست مدل‌ها با <code><span dir="ltr">GET /api/v1/models</span></code>
- **قالب خطا**: شیء <code>error</code> شامل <code>message</code>، <code>type</code>، <code>code</code> و در برخی موارد هدر <code><span dir="ltr">X-Provider-Error</span></code>.

<details>
<summary>نمونه درخواست‌ها (cURL)</summary>

```bash
curl -s -H "Authorization: Bearer $API_KEY" \
     "https://rahyana.ir/api/v1/models"

curl -s -X POST "https://rahyana.ir/api/v1/chat/completions" \
     -H "Authorization: Bearer $API_KEY" \
     -H "Content-Type: application/json" \
     -d '{
       "model": "openai/gpt-4o",
       "messages": [{"role":"user","content":"سلام"}]
     }'
```

</details>

## 📚 مخازن زبان‌ها
- JavaScript: به‌زودی اضافه می‌شود
- TypeScript: به‌زودی اضافه می‌شود
- Python: به‌زودی اضافه می‌شود

## 🧩 چه چیزهایی پیدا می‌کنید؟
- مثال‌های «چت تکمیلی» (Basic/Streaming/JSON Mode) و ورودی‌های تصویر/صوت/PDF
- پروژه‌های واقعی و پرتقاضا (تولید محتوا، چت‌بات، دستیار کدنویسی و ...)
- ابزارهای توسعه‌محور (تولید تست، مانیتورینگ عملکرد، تولید مستندات، بازبین کد، CI/CD)

## ✅ استانداردهای کیفیت
- مثال‌ها «قابل اجرا» و مستند هستند (FA/EN)
- تست دود (Smoke Test) برای اطمینان از صحت اجرای نمونه‌ها
- فرمت و لینت استاندارد (Black/Ruff، ESLint/Prettier)

## 🤝 مشارکت
- باگ یا پیشنهاد دارید؟ در «Issues» مطرح کنید.
- ایده‌های جدید را در «Discussions» به اشتراک بگذارید.
- راهنمای مشارکت: فایل `CONTRIBUTING.md`

---

<!-- SEO: کلمات کلیدی -->
<!-- Rahyana AI، مثال هوش مصنوعی، GPT-5، GPT-4o، آموزش هوش مصنوعی، چت‌بات، تولید محتوا، Python، TypeScript، JavaScript، OpenAI-compatible, JSON Mode, استریم -->

</div>
