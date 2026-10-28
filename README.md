<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#101010">
<title>Alex SHOP | فروشگاه آنلاین</title>

<style>
:root {
  --bg: #0b0b0d;
  --panel: #17171b;
  --gold: #f4c542;
  --gold2: #ffdf7a;
  --text: #f7f7f7;
  --muted: #b8b8c0;
  --line: #33333b;
}

* {
  box-sizing: border-box;
}

body {
  margin: 0;
  background: radial-gradient(
    circle at top,
    #252015 0,
    #101012 34%,
    var(--bg) 75%
  );
  color: var(--text);
  font-family: Tahoma, Arial, sans-serif;
  line-height: 1.8;
}

button, input {
  font: inherit;
}

button {
  cursor: pointer;
}

.wrap {
  width: min(1100px, 94%);
  margin: auto;
}

header {
  padding: 28px 0 22px;
  text-align: center;
}

.brand {
  font-size: clamp(30px, 6vw, 48px);
  font-weight: 900;
  color: var(--gold);
  margin: 0;
  text-shadow: 0 0 25px #f4c54233;
}

.subtitle {
  margin: 4px 0;
  color: var(--muted);
}

.badge {
  display: inline-block;
  border: 1px solid #6e5a20;
  color: var(--gold2);
  border-radius: 999px;
  padding: 3px 13px;
  font-size: 12px;
  margin-top: 8px;
}

.hero {
  border: 1px solid #55451d;
  background: linear-gradient(
    120deg,
    #242016,
    #151519 65%,
    #222018
  );
  border-radius: 22px;
  padding: 22px;
  margin: 10px 0 24px;
  text-align: center;
  box-shadow: 0 12px 45px #0005;
}

.hero h2 {
  margin: 0 0 6px;
  font-size: clamp(20px, 4vw, 30px);
}

.hero p {
  margin: 0;
  color: var(--muted);
}

.section-title {
  font-size: 21px;
  margin: 24px 0 12px;
}

.categories {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 13px;
}

.category {
  border: 1px solid var(--line);
  border-radius: 18px;
  padding: 20px 10px;
  background: linear-gradient(145deg, #1c1c21, #111114);
  color: var(--text);
  text-align: center;
  transition: .2s;
}

.category:hover,
.category.active {
  border-color: var(--gold);
  transform: translateY(-2px);
  box-shadow: 0 8px 25px #f4c54212;
}

.category .emoji {
  font-size: 38px;
  display: block;
}

.category strong {
  display: block;
  color: var(--gold2);
  font-size: 16px;
}

.category small {
  color: var(--muted);
}

.toolbar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 10px;
  flex-wrap: wrap;
  margin: 24px 0 12px;
}

.toolbar h2 {
  margin: 0;
  font-size: 21px;
}

.count {
  font-size: 12px;
  color: var(--muted);
}

.products {
  display: grid;
  grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 13px;
}

.product {
  background: linear-gradient(145deg, #1a1a1f, #121215);
  border: 1px solid var(--line);
  border-radius: 17px;
  padding: 16px;
  display: flex;
  flex-direction: column;
  min-width: 0;
}

.product .picon {
  font-size: 30px;
}

.product h3 {
  font-size: 16px;
  margin: 5px 0 7px;
  line-height: 1.7;
}

.price {
  color: var(--gold2);
  font-weight: bold;
  font-size: 17px;
  margin: 0 0 12px;
}

.hint {
  color: var(--muted);
  font-size: 12px;
  margin: auto 0 12px;
}

.primary,
.secondary,
.copybtn {
  border: 0;
  border-radius: 10px;
  padding: 10px 13px;
  font-weight: bold;
}

.primary {
  background: linear-gradient(120deg, var(--gold), var(--gold2));
  color: #17130a;
}

.secondary {
  background: #292930;
  color: var(--text);
  border: 1px solid #44444d;
}

.primary:active,
.secondary:active,
.copybtn:active {
  transform: scale(.98);
}

.product .primary {
  width: 100%;
}

.notice {
  background: #211d11;
  border: 1px solid #57471c;
  border-radius: 13px;
  padding: 12px 14px;
  color: #e7d8a8;
  font-size: 12px;
  margin: 20px 0;
}

footer {
  text-align: center;
  color: var(--muted);
  padding: 25px 0 35px;
  font-size: 12px;
}

@media (max-width: 760px) {
  .products {
    grid-template-columns: repeat(2, minmax(0, 1fr));
  }

  .categories {
    gap: 8px;
  }

  .category {
    padding: 16px 6px;
  }

  .category .emoji {
    font-size: 31px;
  }

  .category strong {
    font-size: 14px;
  }
}

@media (max-width: 420px) {
  .products {
    grid-template-columns: 1fr 1fr;
  }

  .product {
    padding: 12px;
  }

  .product h3 {
    font-size: 14px;
  }

  .price {
    font-size: 15px;
  }

  .categories {
    grid-template-columns: 1fr;
  }

  .category {
    display: flex;
    align-items: center;
    gap: 12px;
    text-align: right;
    padding: 12px 16px;
  }

  .category .emoji {
    width: 42px;
  }

  .category strong {
    font-size: 15px;
  }
}
</style></head>
<body>

<header class="wrap">
  <h1 class="brand">𝗔𝗹𝗲𝘅 𝗦𝗛𝗢𝗣</h1>
  <p class="subtitle">فروشگاه آنلاین خدمات و محصولات دیجیتال</p>
  <span class="badge">سفارش آسان • پرداخت کارت‌به‌کارت</span>
</header>

<main class="wrap">

  <section class="hero">
    <h2>به فروشگاه الکس خوش آمدید ✨</h2>
    <p>دسته‌بندی موردنظر خود را انتخاب کنید و محصول را سفارش دهید.</p>
  </section>

  <h2 class="section-title">دسته‌بندی محصولات</h2>

  <section class="categories">

    <button class="category active"
      data-category="ff"
      onclick="showCategory('ff')">

      <span class="emoji">💎</span>

      <span>
        <strong>الماس فری فایر</strong>
        <small>شارژ با آیدی</small>
      </span>

    </button>

    <button class="category"
      data-category="pubg"
      onclick="showCategory('pubg')">

      <span class="emoji">🎮</span>

      <span>
        <strong>یوسی پابجی موبایل</strong>
        <small>شارژ با آیدی</small>
      </span>

    </button>

    <button class="category"
      data-category="kafing"
      onclick="showCategory('kafing')">

      <span class="emoji">🌐</span>

      <span>
        <strong>کافینگ ویتوری</strong>
        <small>بسته‌های اینترنت</small>
      </span>

    </button>

  </section>

  <div class="toolbar">
    <h2 id="productsTitle">💎 محصولات فری فایر</h2>
    <span class="count" id="productsCount"></span>
  </div>

  <section class="products" id="products"></section>

  <div class="notice">
    ⚠️ پس از انتقال وجه، روی «واریز کردم» بزنید و پیام آماده‌شده را در روبیکا ارسال کنید.
    ثبت این پیام به‌تنهایی تأیید پرداخت نیست؛ سفارش پس از بررسی واریز تأیید می‌شود.
  </div>

</main>

<footer class="wrap">
  © Alex SHOP — تمامی حقوق محفوظ است.
</footer><div class="modal-backdrop" id="modalBackdrop"
     role="dialog" aria-modal="true"
     aria-labelledby="modalTitle">

  <div class="modal">

    <div class="modal-head">
      <div>
        <h2 id="modalTitle">ثبت سفارش</h2>
        <div class="count" id="modalProductLabel"></div>
      </div>

      <button class="close" onclick="closeModal()">
        بستن ✕
      </button>
    </div>

    <div class="field" id="idField">
      <label for="customerId" id="customerIdLabel">
        آیدی بازیکن
      </label>

      <input id="customerId"
             autocomplete="off"
             placeholder="آیدی خود را وارد کنید">
    </div>

    <div class="field" id="nameField">
      <label for="customerName">
        نام یا نام کاربری شما (اختیاری)
      </label>

      <input id="customerName"
             autocomplete="name"
             placeholder="نام شما">
    </div>

    <div class="payment-box">

      <div class="payrow">
        <div>
          <div class="label">نام محصول</div>
          <div class="value" id="payProduct"></div>
        </div>

        <button class="copybtn"
          onclick="copyText(document.getElementById('payProduct').textContent)">
          کپی
        </button>
      </div>

      <div class="payrow">
        <div>
          <div class="label">مبلغ قابل پرداخت</div>
          <div class="value total" id="payAmount"></div>
        </div>

        <button class="copybtn"
          onclick="copyText(document.getElementById('payAmountRaw').value)">
          کپی مبلغ
        </button>
      </div>

      <div class="payrow">
        <div>
          <div class="label">شماره کارت</div>
          <div class="value" id="payCard"></div>
        </div>

        <button class="copybtn"
          onclick="copyText('6277601460171273')">
          کپی شماره کارت
        </button>
      </div>

      <div class="payrow">
        <div>
          <div class="label">نام صاحب کارت</div>
          <div class="value" id="payOwner">شاوردی</div>
        </div>

        <button class="copybtn"
          onclick="copyText('شاوردی')">
          کپی نام
        </button>
      </div>

    </div>

    <input type="hidden" id="payAmountRaw">

    <div class="modal-actions">

      <button class="primary" onclick="markPaid()">
        ✅ واریز کردم
      </button>

      <button class="secondary" onclick="closeModal()">
        بازگشت به محصولات
      </button>

    </div>

    <p class="count">
      با زدن «واریز کردم»، متن سفارش کپی می‌شود و صفحه روبیکا باز خواهد شد.
      برای ارسال سفارش، پیام را در روبیکا ارسال کنید.
    </p>

  </div>
</div>

<div id="toast" role="status"></div><script>
/* إعدادات المتجر */
const CARD_NUMBER = "6277601460171273";
const CARD_OWNER = "شاوردی";
const RUBIKA_PROFILE = "https://rubika.ir/FA_RIli";

/* جميع المنتجات والأسعار بالريال الإيراني */
const productsData = {

  ff: [
    {name:"۱۱۰ الماس فری فایر",price:2800000,detail:"شارژ با آیدی"},
    {name:"۲۲۰ الماس فری فایر",price:5480000,detail:"شارژ با آیدی"},
    {name:"۳۴۱ الماس فری فایر",price:8120000,detail:"شارژ با آیدی"},
    {name:"۴۵۱ الماس فری فایر",price:10870000,detail:"شارژ با آیدی"},
    {name:"۵۷۲ الماس فری فایر",price:13590000,detail:"شارژ با آیدی"},
    {name:"۷۹۲ الماس فری فایر",price:18980000,detail:"شارژ با آیدی"},
    {name:"۱۰۲۳ الماس فری فایر",price:24480000,detail:"شارژ با آیدی"},
    {name:"۱۱۶۶ الماس فری فایر",price:27120000,detail:"شارژ با آیدی"},
    {name:"۱۷۳۸ الماس فری فایر",price:40720000,detail:"شارژ با آیدی"},
    {name:"۲۳۸۸ الماس فری فایر",price:54020000,detail:"شارژ با آیدی"},
    {name:"کارت هفتگی لایت",price:1750000,detail:"نیازمند اطلاعات حساب"},
    {name:"کارت هفتگی",price:4800000,detail:"نیازمند اطلاعات حساب"},
    {name:"کارت ماهانه",price:27220000,detail:"شارژ با آیدی"}
  ],

  pubg: [
    {name:"۳۰ یوسی پابجی موبایل",price:1810000,detail:"شارژ با آیدی"},
    {name:"۶۰ یوسی پابجی موبایل",price:2810000,detail:"شارژ با آیدی"},
    {name:"۱۲۰ یوسی پابجی موبایل",price:5200000,detail:"شارژ با آیدی"},
    {name:"۱۸۰ یوسی پابجی موبایل",price:7580000,detail:"شارژ با آیدی"},
    {name:"۳۲۵ یوسی پابجی موبایل",price:12570000,detail:"شارژ با آیدی"},
    {name:"۳۸۵ یوسی پابجی موبایل",price:15480000,detail:"شارژ با آیدی"},
    {name:"۶۶۰ یوسی پابجی موبایل",price:25450000,detail:"شارژ با آیدی"},
    {name:"۷۲۰ یوسی پابجی موبایل",price:27820000,detail:"شارژ با آیدی"}
  ],

  kafing: [
    {name:"بسته ۱۰ گیگابایت — ۳۰ روزه — کاربر نامحدود",price:1200000,detail:"بسته اینترنت"},
    {name:"بسته ۲۰ گیگابایت — ۳۰ روزه — کاربر نامحدود",price:1650000,detail:"بسته اینترنت"},
    {name:"بسته ۳۰ گیگابایت — ۳۰ روزه — کاربر نامحدود",price:2200000,detail:"بسته اینترنت"},
    {name:"بسته ۵۰ گیگابایت — ۳۰ روزه — کاربر نامحدود",price:3100000,detail:"بسته اینترنت"}
  ]

};/* ================================
   الجزء الخامس: وظائف المتجر
================================ */

/* تنسيق نافذة الطلب */
const modalStyles = document.createElement("style");

modalStyles.textContent = `
.modal-backdrop {
  display: none;
  position: fixed;
  inset: 0;
  z-index: 9999;
  background: rgba(0,0,0,.82);
  padding: 16px;
  overflow-y: auto;
  align-items: center;
  justify-content: center;
}

.modal-backdrop.open {
  display: flex;
}

.modal {
  background: #17171b;
  border: 1px solid #6e5a20;
  border-radius: 18px;
  padding: 20px;
  width: min(100%, 500px);
  max-height: 92vh;
  overflow-y: auto;
  box-shadow: 0 15px 50px #0009;
}

.modal-head,
.payrow {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 12px;
}

.modal-head {
  margin-bottom: 20px;
}

.modal-head h2 {
  margin: 0;
  color: #ffdf7a;
}

.close {
  background: #292930;
  color: #fff;
  border: 1px solid #44444d;
  border-radius: 9px;
  padding: 8px 12px;
}

.field {
  margin-bottom: 16px;
}

.field label,
.label {
  display: block;
  color: #b8b8c0;
  font-size: 13px;
  margin-bottom: 5px;
}

.field input {
  width: 100%;
  padding: 12px;
  background: #0b0b0d;
  color: #fff;
  border: 1px solid #44444d;
  border-radius: 10px;
  outline: none;
}

.field input:focus {
  border-color: #f4c542;
}

.payment-box {
  background: #101012;
  border: 1px solid #33333b;
  border-radius: 12px;
  padding: 12px;
  margin: 18px 0;
}

.payrow {
  padding: 12px 0;
  border-bottom: 1px solid #33333b;
}

.payrow:last-child {
  border-bottom: 0;
}

.value {
  font-weight: bold;
  overflow-wrap: anywhere;
}

.total {
  color: #ffdf7a;
  font-size: 18px;
}

.copybtn {
  background: #292930;
  color: #ffdf7a;
  border: 1px solid #44444d;
  white-space: nowrap;
}

.modal-actions {
  display: grid;
  gap: 10px;
  margin: 18px 0;
}

.modal-actions button {
  width: 100%;
}

#toast {
  position: fixed;
  bottom: 20px;
  left: 50%;
  transform: translateX(-50%);
  z-index: 10000;
  background: #242016;
  color: #ffdf7a;
  border: 1px solid #6e5a20;
  border-radius: 10px;
  padding: 10px 16px;
  display: none;
  max-width: 90%;
  text-align: center;
}

#toast.show {
  display: block;
}

@media (max-width: 420px) {
  .modal {
    padding: 14px;
  }

  .payrow {
    align-items: flex-start;
  }
}
`;

document.head.appendChild(modalStyles);

/* متغيرات المتجر */
let currentCategory = "ff";
let selectedProduct = null;
let selectedCategory = "ff";

/* أسماء الأقسام */
const categoryNames = {
  ff: "💎 محصولات فری فایر",
  pubg: "🎮 محصولات پابجی موبایل",
  kafing: "🌐 بسته‌های اینترنت"
};

/* تنسيق السعر */
function formatPrice(price) {
  return new Intl.NumberFormat("fa-IR").format(price) + " ریال";
}

/* عرض رسالة صغيرة */
let toastTimer;

function showToast(message) {
  const toast = document.getElementById("toast");

  toast.textContent = message;
  toast.classList.add("show");

  clearTimeout(toastTimer);

  toastTimer = setTimeout(() => {
    toast.classList.remove("show");
  }, 2500);
}

/* نسخ النص */
async function copyText(text) {
  try {
    if (navigator.clipboard && window.isSecureContext) {
      await navigator.clipboard.writeText(String(text));
    } else {
      const area = document.createElement("textarea");

      area.value = String(text);
      area.style.position = "fixed";
      area.style.opacity = "0";

      document.body.appendChild(area);
      area.select();

      const copied = document.execCommand("copy");
      area.remove();

      if (!copied) {
        throw new Error("copy failed");
      }
    }

    showToast("✅ کپی شد");
  } catch (error) {
    showToast("کپی خودکار انجام نشد؛ متن را دستی کپی کنید.");
  }
}

/* عرض المنتجات */
function renderProducts(category) {
  const container = document.getElementById("products");
  const title = document.getElementById("productsTitle");
  const count = document.getElementById("productsCount");

  if (!container || !productsData[category]) {
    return;
  }

  currentCategory = category;

  title.textContent = categoryNames[category];
  count.textContent =
    new Intl.NumberFormat("fa-IR").format(
      productsData[category].length
    ) + " محصول";

  container.innerHTML = "";

  productsData[category].forEach((product, index) => {
    const card = document.createElement("article");
    card.className = "product";

    let icon = "🌐";

    if (category === "ff") {
      icon = "💎";
    } else if (category === "pubg") {
      icon = "🎮";
    }

    const iconElement = document.createElement("div");
    iconElement.className = "picon";
    iconElement.textContent = icon;

    const name = document.createElement("h3");
    name.textContent = product.name;

    const price = document.createElement("p");
    price.className = "price";
    price.textContent = formatPrice(product.price);

    const hint = document.createElement("p");
    hint.className = "hint";
    hint.textContent = product.detail;

    const button = document.createElement("button");
    button.className = "primary";
    button.textContent = "🛒 سفارش محصول";

    button.addEventListener("click", () => {
      openModal(category, index);
    });

    card.append(
      iconElement,
      name,
      price,
      hint,
      button
    );

    container.appendChild(card);
  });

  document.querySelectorAll(".category").forEach(button => {
    button.classList.toggle(
      "active",
      button.dataset.category === category
    );
  });
}

/* تبديل القسم */
function showCategory(category) {
  if (!productsData[category]) {
    return;
  }

  renderProducts(category);
}

/* فتح نافذة الطلب */
function openModal(category, index) {
  const product = productsData[category]?.[index];

  if (!product) {
    showToast("تعذر العثور على المنتج.");
    return;
  }

  selectedProduct = product;
  selectedCategory = category;

  document.getElementById("modalProductLabel").textContent =
    product.name;

  document.getElementById("payProduct").textContent =
    product.name;

  document.getElementById("payAmount").textContent =
    formatPrice(product.price);

  document.getElementById("payAmountRaw").value =
    String(product.price);

  document.getElementById("payCard").textContent =
    CARD_NUMBER;

  document.getElementById("payOwner").textContent =
    CARD_OWNER;

  const idField = document.getElementById("idField");
  const idLabel = document.getElementById("customerIdLabel");
  const customerId = document.getElementById("customerId");

  if (category === "kafing") {
    idLabel.textContent = "اطلاعات موردنیاز برای بسته اینترنت";
    customerId.placeholder = "اطلاعات لازم را وارد کنید";
  } else {
    idLabel.textContent = "آیدی بازیکن";
    customerId.placeholder = "آیدی خود را وارد کنید";
  }

  idField.style.display = "block";

  document.getElementById("customerId").value = "";
  document.getElementById("customerName").value = "";

  document.getElementById("modalBackdrop").classList.add("open");

  document.body.style.overflow = "hidden";
}

/* بستن نافذة الطلب */
function closeModal() {
  document.getElementById("modalBackdrop").classList.remove("open");

  document.body.style.overflow = "";
}

/* إغلاق النافذة عند الضغط على الخلفية */
document.getElementById("modalBackdrop").addEventListener(
  "click",
  function(event) {
    if (event.target === this) {
      closeModal();
    }
  }
);

/* إغلاق النافذة بزر Escape */
document.addEventListener("keydown", function(event) {
  if (event.key === "Escape") {
    closeModal();
  }
});

/* تجهيز رسالة الطلب وفتح روبیکا */
function markPaid() {
  if (!selectedProduct) {
    showToast("يرجى اختيار منتج أولاً.");
    return;
  }

  const customerId =
    document.getElementById("customerId").value.trim();

  const customerName =
    document.getElementById("customerName").value.trim();

  if (!customerId) {
    showToast("يرجى إدخال المعلومات المطلوبة.");
    document.getElementById("customerId").focus();
    return;
  }

  const categoryLabels = {
    ff: "فری فایر",
    pubg: "پابجی موبایل",
    kafing: "بسته اینترنت"
  };

  const message = [
    "🛍️ سفارش جدید | Alex SHOP",
    "━━━━━━━━━━━━━━",
    "📦 محصول: " + selectedProduct.name,
    "🎮 القسم: " + categoryLabels[selectedCategory],
    "💰 المبلغ: " + formatPrice(selectedProduct.price),
    "🆔 آيدي اللاعب / المعلومات: " + customerId,
    "👤 اسم المشتري: " + (customerName || "لم يذكر"),
    "💳 رقم البطاقة: " + CARD_NUMBER,
    "👑 صاحب البطاقة: " + CARD_OWNER,
    "━━━━━━━━━━━━━━",
    "⚠️ حالة الدفع: بانتظار التحقق من البائع",
    "📌 يرجى التحقق من الدفع قبل تنفيذ الطلب."
  ].join("\n");

  copyText(message);

  showToast("تم تجهيز الطلب؛ أرسل الرسالة في روبیکا.");

  closeModal();

  setTimeout(() => {
    window.location.href = RUBIKA_PROFILE;
  }, 700);
}

/* تشغيل المتجر وعرض المنتجات */
renderProducts("ff");
</script>

</body>
</html>
