
# EduVerify 🎓

> A mobile platform for academic enrollment and document verification using OCR technology.

![Flutter](https://img.shields.io/badge/Flutter-02569B?style=for-the-badge&logo=flutter&logoColor=white)
![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)

---

## 📌 Overview

**EduVerify** is a mobile application that streamlines the student enrollment process by allowing students to digitally submit their academic documents — national ID (CIN), baccalaureate certificate, and transcripts — for automated OCR-based extraction and manual review by academic institutions.

Built as an academic project at **EMSI Marrakech** (March 2025 – June 2025).

---

## ✨ Features

### 👨‍🎓 Student Side
- Step-by-step document submission flow (CIN recto/verso, Baccalaureate, Transcripts)
- Real-time verification progress tracking with global completion percentage
- Per-document status tracking: **Verified**, **Pending**, **To Revise**
- Instant notifications on document status changes
- Personalized dashboard with institution details and last update timestamp

### 🏫 Admin / Institution Side
- Dashboard to review all submitted student documents
- Manual approval, rejection, or revision request per document
- OCR-powered automatic extraction and pre-validation of student information
- Multi-stage verification pipeline management

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|------------|
| Mobile | Flutter (Dart) |
| Backend | Laravel (PHP) |
| Database | MySQL |
| API | REST API |
| OCR | Optical Character Recognition |

---

## 📱 Screenshots

<img width="200" height="500" alt="ChatGPT Image 22 juin 2026, 16_37_18" src="https://github.com/user-attachments/assets/40609c67-f997-4e82-bc33-d22dac6234df" />

<img width="200" height="500" alt="ChatGPT Image 22 juin 2026, 16_37_29" src="https://github.com/user-attachments/assets/0515e4ab-5b05-4c36-a355-1f00e8ce7409" />


<img width="200" height="500" alt="ChatGPT Image 22 juin 2026, 16_37_38" src="https://github.com/user-attachments/assets/1c286a5c-20f3-4681-8b93-0d77f118ef51" />

---

## 🚀 Getting Started

### Prerequisites

- PHP 8.1+
- Composer
- Laravel 10+
- MySQL
- Flutter SDK 3.0+
- Android Studio / Xcode

---

## 🔌 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/api/auth/register` | Student registration |
| `POST` | `/api/auth/login` | Authentication |
| `POST` | `/api/documents/upload` | Upload a document |
| `GET` | `/api/documents` | Get all student documents |
| `GET` | `/api/documents/{id}/status` | Get document verification status |
| `GET` | `/api/verification/progress` | Get global verification progress |
| `PUT` | `/api/admin/documents/{id}/review` | Admin: review a document |
