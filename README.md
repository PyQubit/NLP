# 🤖 NLP with Deep Learning — IMDB Sentiment Analysis

> **Deep learning for sentiment classification of movie reviews using LSTM.**
> **تحلیل احساسات نقدهای فیلم با استفاده از یادگیری عمیق و شبکه LSTM.**

---

## 📌 Table of Contents | فهرست مطالب

* [👋 Introduction | مقدمه](#-introduction--مقدمه)
* [🚀 Features | قابلیت‌ها](#-features--قابلیت‌ها)
* [🧠 Model Architecture | معماری مدل](#-model-architecture--معماری-مدل)
* [📂 Dataset | دیتاست](#-dataset--دیتاست)
* [📊 Results | نتایج](#-results--نتایج)
* [⚙️ Requirements | پیش‌نیازها](#️-requirements--پیشنیازها)
* [📥 Installation & Usage | نصب و اجرا](#-installation--usage--نصب-و-اجرا)
* [🐞 Troubleshooting | رفع خطا](#-troubleshooting--رفع-خطا)
* [👤 Developer | توسعه‌دهنده](#-developer--توسعهدهنده)
* [📄 License | مجوز](#-license--مجوز)

---

<a id="-introduction--مقدمه"></a>

## 👋 Introduction | مقدمه

### 🇬🇧 English

This project demonstrates **Natural Language Processing (NLP) with Deep Learning** using an **LSTM-based Recurrent Neural Network (RNN)** for binary sentiment classification.

The model is trained on the well-known **IMDB Movie Reviews dataset** and learns to classify reviews into positive and negative sentiment categories.

The project covers the complete workflow from text preprocessing and sequence preparation to model training, evaluation, and visualization.

### 🇮🇷 فارسی

این پروژه نمونه‌ای از **پردازش زبان طبیعی (NLP) با یادگیری عمیق** است که در آن از یک **شبکه بازگشتی مبتنی بر LSTM** برای طبقه‌بندی دودویی احساسات استفاده می‌شود.

مدل روی دیتاست معروف **IMDB Movie Reviews** آموزش داده شده و یاد می‌گیرد نقدهای فیلم را در دو دسته مثبت و منفی طبقه‌بندی کند.

این پروژه فرایند کامل پردازش متن، آماده‌سازی دنباله‌ها، آموزش مدل، ارزیابی و نمایش نتایج را پوشش می‌دهد.

---

<a id="-features--قابلیت‌ها"></a>

## 🚀 Features | قابلیت‌ها

* 🧹 **Text Preprocessing** — پیش‌پردازش داده‌های متنی
* 🔤 **Word Index Mapping** — تبدیل واژه‌ها به شناسه‌های عددی
* 📏 **Sequence Padding** — یکسان‌سازی طول دنباله‌های متنی
* 🧠 **LSTM-based Classification** — طبقه‌بندی احساسات با LSTM
* 🎯 **Binary Sentiment Analysis** — تشخیص احساس مثبت و منفی
* 📚 **Model Training** — آموزش مدل یادگیری عمیق
* 📊 **Model Evaluation** — ارزیابی عملکرد روی داده‌های تست
* ☁️ **WordCloud Visualization** — نمایش کلمات پرتکرار
* 📈 **Matplotlib Visualization** — نمایش و تحلیل نتایج آموزشی

---

<a id="-model-architecture--معماری-مدل"></a>

## 🧠 Model Architecture | معماری مدل

### 🇬🇧 English

The project uses an **LSTM-based RNN architecture** for processing sequential text data.

```text
IMDB Movie Review
       │
       ▼
Text Preprocessing
       │
       ▼
Word Index Mapping
       │
       ▼
Sequence Padding
       │
       ▼
Embedding
       │
       ▼
LSTM
       │
       ▼
Dense Output Layer
       │
       ▼
Positive / Negative
```

### 🇮🇷 فارسی

معماری پروژه بر پایه شبکه بازگشتی **LSTM** برای پردازش داده‌های متنی ترتیبی است:

```text
نقد فیلم IMDB
       │
       ▼
پیش‌پردازش متن
       │
       ▼
نگاشت واژه‌ها به شناسه
       │
       ▼
Padding دنباله‌ها
       │
       ▼
Embedding
       │
       ▼
LSTM
       │
       ▼
لایه خروجی Dense
       │
       ▼
مثبت / منفی
```

---

<a id="-dataset--دیتاست"></a>

## 📂 Dataset | دیتاست

### 🇬🇧 English

The project uses the **IMDB Movie Reviews dataset** provided through `keras.datasets`.

The dataset contains movie reviews labeled for binary sentiment classification:

* **Positive**
* **Negative**

The dataset is automatically loaded through Keras and does not need to be manually downloaded.

### 🇮🇷 فارسی

در این پروژه از دیتاست **IMDB Movie Reviews** موجود در `keras.datasets` استفاده می‌شود.

داده‌ها برای طبقه‌بندی دودویی احساسات به دو دسته تقسیم شده‌اند:

* **Positive | مثبت**
* **Negative | منفی**

دیتاست از طریق Keras بارگذاری می‌شود و نیازی به دانلود دستی ندارد.

---

<a id="-results--نتایج"></a>

## 📊 Results | نتایج

### 🇬🇧 English

The trained model is evaluated on the IMDB test set.

The notebook also provides visualizations for analyzing the training process and text data, including:

* Training / validation metrics
* Evaluation results
* WordCloud visualizations
* Frequently occurring words

### 🇮🇷 فارسی

مدل آموزش‌دیده روی مجموعه داده تست IMDB ارزیابی می‌شود.

همچنین نوت‌بوک شامل نمودارها و نمایش‌های بصری برای بررسی فرایند آموزش و داده‌های متنی است، از جمله:

* معیارهای آموزش و اعتبارسنجی
* نتایج ارزیابی
* ابر واژه‌ها
* کلمات پرتکرار

> **Note | توجه:** اعداد دقیق عملکرد مدل باید مستقیماً از خروجی اجرای نهایی Notebook استخراج شوند و در صورت نیاز در این بخش اضافه شوند.

---

<a id="️-requirements--پیشنیازها"></a>

## ⚙️ Requirements | پیش‌نیازها

> ⚠️ **Python 3.8.8 is recommended for the original project environment.**
> ⚠️ **برای محیط اصلی این پروژه استفاده از Python 3.8.8 توصیه می‌شود.**

### Dependencies | کتابخانه‌ها

```bash
pip install tensorflow keras numpy matplotlib wordcloud jupyter
```

---

<a id="-installation--usage--نصب-و-اجرا"></a>

## 📥 Installation & Usage | نصب و اجرا

### 1. Clone the Repository | دریافت پروژه

```bash
git clone https://github.com/PyQubit/NLP.git
cd NLP
```

### 2. Create a Virtual Environment | ساخت محیط مجازی

```bash
python -m venv env
```

**Windows:**

```bash
.\env\Scripts\activate
```

**Linux / macOS:**

```bash
source env/bin/activate
```

### 3. Install Dependencies | نصب وابستگی‌ها

```bash
pip install tensorflow keras numpy matplotlib wordcloud jupyter
```

### 4. Launch Jupyter Notebook | اجرای Jupyter Notebook

```bash
jupyter notebook
```

Then open:

```text
NLP.ipynb
```

سپس فایل `NLP.ipynb` را باز کرده و سلول‌های Notebook را اجرا کنید.

---

<a id="-troubleshooting--رفع-خطا"></a>

## 🐞 Troubleshooting | رفع خطا

### `ModuleNotFoundError`

Install the required dependencies:

```bash
pip install tensorflow keras numpy matplotlib wordcloud jupyter
```

### TensorFlow / Python Compatibility Issues

If you encounter compatibility problems, use the original recommended environment:

```text
Python 3.8.8
```

Using a compatible TensorFlow version may also be necessary depending on the operating system.

---

<a id="-developer--توسعهدهنده"></a>

## 👤 Developer | توسعه‌دهنده

### Mohammad Mahdi Omidvar — PyQubit

**AI Engineer & Data Scientist**

Interested in:

* Artificial Intelligence
* Machine Learning
* Deep Learning
* Natural Language Processing
* Computer Vision
* Data Science

### ارتباط با من

* **GitHub:** https://github.com/PyQubit
* **Portfolio:** https://pyqubit.github.io/
* **Instagram:** https://instagram.com/PyQubit
* **Telegram:** https://t.me/PyQubit
* **Email:** [PyQubit@gmail.com](mailto:PyQubit@gmail.com)

---

<a id="-license--مجوز"></a>

## 📄 License | مجوز

This project is **proprietary software**.

این پروژه یک **نرم‌افزار اختصاصی** است.

© 2025–2026 **Mohammad Mahdi Omidvar (PyQubit)** — All Rights Reserved.

See [`LICENSE`](LICENSE) for the complete terms.

---

<div align="center">

### 🤖 NLP with Deep Learning

**IMDB Sentiment Analysis using LSTM**

</div>

