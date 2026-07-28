💬 Chat Pro

یک پلتفرم چت آنلاین و Real-Time فول‌استک با قابلیت ثبت‌نام، ورود کاربران، اتاق‌های گفتگو، پیام خصوصی، کاربران آنلاین و ارسال فایل و تصویر.

---

🚀 معرفی پروژه

Chat Pro یک پروژه پیام‌رسان آنلاین است که برای یادگیری و توسعه سیستم‌های Real-Time طراحی شده است.

کاربران می‌توانند در این سیستم ثبت‌نام کنند، وارد حساب خود شوند، با سایر کاربران به‌صورت لحظه‌ای گفتگو کنند، وارد اتاق‌های مختلف شوند و فایل یا تصویر ارسال کنند.

---

✨ امکانات پروژه

👤 کاربران

- ثبت‌نام کاربر
- ورود و خروج از حساب
- احراز هویت با JWT
- رمزنگاری رمز عبور
- مدیریت اطلاعات کاربر
- نمایش کاربران آنلاین

💬 چت Real-Time

- ارسال پیام لحظه‌ای
- دریافت پیام بدون Refresh کردن صفحه
- ذخیره پیام‌ها در دیتابیس
- نمایش تاریخچه پیام‌ها
- نمایش وضعیت آنلاین کاربران
- نمایش وضعیت «در حال نوشتن...»

🏠 اتاق‌های گفتگو

- ایجاد اتاق گفتگو
- ورود به اتاق
- خروج از اتاق
- چت گروهی
- مشاهده اعضای اتاق

🔒 پیام خصوصی

- ارسال پیام مستقیم به کاربران
- ایجاد گفتگوی خصوصی
- ذخیره تاریخچه پیام‌های خصوصی

📎 ارسال فایل و تصویر

- ارسال تصاویر
- ارسال فایل
- نمایش تصویر در چت
- دانلود فایل‌های ارسال شده

🎨 رابط کاربری

- طراحی مدرن و واکنش‌گرا
- سازگار با موبایل و دسکتاپ
- طراحی شده با React
- استفاده از Tailwind CSS
- صفحه ورود
- صفحه ثبت‌نام
- صفحه اصلی چت
- Sidebar کاربران و اتاق‌ها

---

🛠 تکنولوژی‌های استفاده شده

Backend

- Node.js
- Express.js
- MongoDB
- Mongoose
- Socket.IO
- JWT
- Bcrypt
- Multer

Frontend

- React
- React Router
- Axios
- Socket.IO Client
- Tailwind CSS

DevOps

- Docker
- Docker Compose
- Nginx

---

📁 ساختار پروژه

chat-pro/
│
├── backend/
│   │
│   ├── src/
│   │   ├── config/
│   │   │   └── database.js
│   │   │
│   │   ├── controllers/
│   │   │   ├── authController.js
│   │   │   ├── userController.js
│   │   │   ├── roomController.js
│   │   │   └── messageController.js
│   │   │
│   │   ├── middleware/
│   │   │   ├── auth.js
│   │   │   ├── upload.js
│   │   │   └── errorHandler.js
│   │   │
│   │   ├── models/
│   │   │   ├── User.js
│   │   │   ├── Room.js
│   │   │   └── Message.js
│   │   │
│   │   ├── routes/
│   │   │   ├── auth.js
│   │   │   ├── users.js
│   │   │   ├── rooms.js
│   │   │   └── messages.js
│   │   │
│   │   ├── socket/
│   │   │   └── socket.js
│   │   │
│   │   └── server.js
│   │
│   ├── uploads/
│   │
│   ├── .env
│   └── package.json
│
├── frontend/
│   │
│   ├── src/
│   │   │
│   │   ├── components/
│   │   │   ├── Sidebar.jsx
│   │   │   ├── ChatWindow.jsx
│   │   │   ├── Message.jsx
│   │   │   ├── UserList.jsx
│   │   │   └── FileUpload.jsx
│   │   │
│   │   ├── pages/
│   │   │   ├── Login.jsx
│   │   │   ├── Register.jsx
│   │   │   └── Chat.jsx
│   │   │
│   │   ├── services/
│   │   │   ├── api.js
│   │   │   └── socket.js
│   │   │
│   │   ├── App.jsx
│   │   └── main.jsx
│   │
│   ├── .env
│   └── package.json
│
├── docker-compose.yml
├── .env.example
├── .gitignore
└── README.md

---

⚙️ نصب و راه‌اندازی

پیش‌نیازها

قبل از اجرای پروژه باید موارد زیر روی سیستم نصب باشند:

- Node.js
- npm
- MongoDB
- Git

یا می‌توانید از Docker استفاده کنید.

---

📥 دریافت پروژه

git clone https://github.com/your-username/chat-pro.git

سپس وارد پوشه پروژه شوید:

cd chat-pro

---

🔧 راه‌اندازی Backend

وارد پوشه Backend شوید:

cd backend

وابستگی‌ها را نصب کنید:

npm install

یک فایل ".env" ایجاد کنید:

PORT=5000

MONGODB_URI=mongodb://localhost:27017/chat-pro

JWT_SECRET=your-super-secret-key

JWT_EXPIRES_IN=15m

REFRESH_TOKEN_SECRET=your-refresh-secret-key

CLIENT_URL=http://localhost:5173

سپس Backend را اجرا کنید:

npm run dev

سرور Backend روی آدرس زیر اجرا می‌شود:

http://localhost:5000

---

🎨 راه‌اندازی Frontend

در یک ترمینال جدید وارد پوشه Frontend شوید:

cd frontend

وابستگی‌ها را نصب کنید:

npm install

سپس پروژه را اجرا کنید:

npm run dev

Frontend معمولاً روی آدرس زیر اجرا می‌شود:

http://localhost:5173

---

🐳 اجرای پروژه با Docker

اگر Docker روی سیستم نصب است، می‌توانید کل پروژه را با دستور زیر اجرا کنید:

docker compose up --build

برای اجرای پروژه در پس‌زمینه:

docker compose up -d --build

برای متوقف کردن سرویس‌ها:

docker compose down

---

🔐 احراز هویت

سیستم احراز هویت پروژه با JWT پیاده‌سازی شده است.

فرآیند ورود به شکل زیر است:

User
  │
  ▼
Login
  │
  ▼
Backend
  │
  ▼
Validate User
  │
  ▼
Generate JWT
  │
  ▼
Send Token
  │
  ▼
Frontend

مسیرهای اصلی احراز هویت:

POST /api/auth/register
POST /api/auth/login
POST /api/auth/refresh
POST /api/auth/logout

---

💬 سیستم Real-Time

ارتباط لحظه‌ای بین کاربران با Socket.IO انجام می‌شود.

فرآیند ارسال پیام:

User A
   │
   │ Send Message
   ▼
Socket.IO Server
   │
   ├──────────────► Database
   │
   ▼
User B

رویدادهای اصلی Socket.IO:

join-room
leave-room
send-message
receive-message
user-online
user-offline
typing
stop-typing

---

🗄️ دیتابیس

پروژه از MongoDB برای ذخیره اطلاعات استفاده می‌کند.

مدل‌های اصلی:

User

اطلاعات کاربران را ذخیره می‌کند.

username
email
password
avatar
status
createdAt

Room

اطلاعات اتاق‌های گفتگو را نگهداری می‌کند.

name
description
owner
members
createdAt

Message

پیام‌های ارسال شده را ذخیره می‌کند.

sender
receiver
room
text
file
createdAt

---

📎 آپلود فایل

برای آپلود فایل از Multer استفاده می‌شود.

فرمت‌های مجاز را می‌توان در تنظیمات پروژه مشخص کرد.

نمونه فایل‌های قابل ارسال:

.jpg
.png
.gif
.pdf
.zip
.docx

توصیه می‌شود در محیط Production فایل‌ها روی سرویس‌هایی مانند فضای ذخیره‌سازی ابری نگهداری شوند.

---

🛡️ نکات امنیتی

برای استفاده واقعی در Production پیشنهاد می‌شود:

- استفاده از HTTPS
- قرار ندادن Secretها داخل Git
- استفاده از فایل ".env"
- محدود کردن حجم فایل‌های آپلودی
- اعتبارسنجی نوع فایل
- استفاده از Rate Limiting
- فعال‌سازی CORS مناسب
- استفاده از Helmet
- اعتبارسنجی اطلاعات ورودی
- هش کردن رمزهای عبور
- استفاده از Refresh Token امن

---

📱 طراحی Responsive

رابط کاربری برای دستگاه‌های مختلف طراحی شده است:

- موبایل
- تبلت
- لپ‌تاپ
- دسکتاپ

---

🚧 قابلیت‌های آینده

در نسخه‌های آینده می‌توان امکانات زیر را اضافه کرد:

- تماس صوتی
- تماس تصویری با WebRTC
- پیام صوتی
- واکنش به پیام‌ها
- Reply به پیام
- ویرایش پیام
- حذف پیام
- جستجوی پیام‌ها
- اعلان Push
- حالت Dark Mode
- رمزنگاری End-to-End
- سیستم گزارش و مسدود کردن کاربران
- پنل مدیریت کامل
- سیستم نقش‌ها و دسترسی‌ها

---

🤝 مشارکت در پروژه

برای مشارکت در پروژه:

1. پروژه را Fork کنید.
2. یک Branch جدید ایجاد کنید.
3. تغییرات خود را اعمال کنید.
4. Commit ایجاد کنید.
5. یک Pull Request ارسال کنید.

---

📄 مجوز

این پروژه تحت مجوز MIT منتشر شده است.

---

👨‍💻 توسعه‌دهنده

ساخته شده با ❤️ برای یادگیری و توسعه سیستم‌های Real-Time و Full-Stack.

---

⭐ اگر پروژه برایت مفید بود

با دادن یک Star به پروژه در GitHub از توسعه آن حمایت کنید.