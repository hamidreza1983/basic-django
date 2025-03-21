# 🚀 Django + Docker + PostgreSQL Starter

یک پروژه ساده برای شروع سریع با جنگو، داکر و دیتابیس PostgreSQL. این پروژه به شما کمک می‌کند تا محیط توسعه خود را به راحتی راه‌اندازی کنید.

---

## ✨ ویژگی‌ها
- استفاده از **Docker** برای مدیریت سرویس‌ها
- پایگاه داده **PostgreSQL**
- مدیریت آسان با **docker compose**
- دارای محیط توسعه مجزا

---

## 🛠 پیش‌نیازها
قبل از شروع، مطمئن شوید که ابزارهای زیر نصب شده‌اند:
- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/install/)

---

## 🚦 راه‌اندازی پروژه

1. کد را کلون کنید:
```bash
git clone https://github.com/basic-django.git
cd basic-django
```

2. فایل `.env` را تنظیم کنید:
```bash
nano .env
```

3. کانتینرها را اجرا کنید:
```bash
docker compose up -d
```

4. اجرای مهاجرت‌ها:
```bash
docker compose exec django python manage.py makemigration
docker compose exec django python manage.py migrate
```

5. ایجاد سوپر یوزر:
```bash
docker compose exec django python manage.py createsuperuser
```

6. دسترسی به پروژه در مرورگر:
```bash
http://localhost:8000/admin
```

---
7. استتیک فایلهای خود را درون پوشه استتیک قرار دهید و در پوشه تمپلیت نیز آدرس های اچ تی ام ال را بگذارید

## ⚙️ دستورات کاربردی

- مشاهده لاگ‌ها:
```bash
docker compose logs -f django
```
- ورود به شل جنگو:
```bash
docker compose exec django python manage.py shell
```

---

## 📎 لینک‌های مفید
- [مستندات جنگو](https://docs.djangoproject.com/en/stable/)
- [مستندات PostgreSQL](https://www.postgresql.org/docs/)
- [مستندات Docker](https://docs.docker.com/)

---

✨ با عشق ساخته شده ❤️

