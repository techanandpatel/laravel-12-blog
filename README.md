# 🌐 Laravel 12 Blog Application

A modern **Laravel 12 Blog** built with **Tailwind CSS**, **Fortify** for authentication, and **Sanctum** for API tokens.  
Supports **SQLite** (default) for development and **MySQL** in production.  
Ideal for multi-author blogs, full-stack learning, or production-ready blogging platforms.

---

## 🚀 Features

### Authentication & User Management
- Registration, login, logout (Fortify)  
- Email verification  
- API token authentication (Sanctum)  
- Role-based access: Admin / Author / User / Guest  
- Profile management (name, email, avatar)

### Blogging
- Create, read, update, delete posts  
- Assign posts to **Categories**  
- Assign multiple **Tags** per post  
- Slug generation for SEO-friendly URLs  
- Image upload / thumbnails  
- Optional: Drafts, scheduled posts

### Interaction
- Commenting with nested replies  
- Like/Reaction system  
- Search and filter posts by title, category, tag, or author  

### Frontend/UI
- Blade templates with **Tailwind CSS**  
- Responsive design and reusable components  
- Pagination and optional dark/light mode  

### API
- REST API for posts, categories, tags, authors, comments  
- Token-based authentication with Sanctum  
- JSON responses  

### Notifications
- Email or in-app notifications for new posts and comments  

---

## 📦 Full Module List

- **User / Authentication** – Registration, login/logout, role-based access, profile  
- **Blog Author** – Author profiles, linked posts, admin management, analytics  
- **Post** – CRUD, Categories, Tags, Slug, Image upload, Drafts  
- **Category** – CRUD, Filter posts, SEO pages  
- **Tag** – CRUD, Assign to posts, Filter posts, SEO pages  
- **Comment** – CRUD, Nested replies, Moderation, Notifications  
- **Like / Reaction** – Like posts, count likes, optional reactions  
- **Search & Filter** – Search by title/content/author, filter by category/tag  
- **Frontend / UI** – Blade + Tailwind, Reusable components, Pagination, Responsive  
- **API** – REST API CRUD, Sanctum authentication, JSON responses  
- **Database / Migrations** – Users, Authors, Posts, Categories, Tags, Comments, Likes  
- **Notifications** – Email/in-app notifications  
- **Analytics / Dashboard** – Admin stats, charts, post/author popularity  
- **Utilities / Helpers** – Slug generator, image upload, validation, pagination, search helpers  

---

## 🗄 Database Structure & Relationships

### Tables
- `users`, `authors`, `posts`, `categories`, `tags`, `comments`, `likes`  

### Relationships
- **User → Post:** One-to-Many  
- **Post → Category:** Many-to-One  
- **Post ↔ Tag:** Many-to-Many  
- **Post → Comment:** One-to-Many  
- **Post → Like:** One-to-Many  

---

## ⚙️ Installation

1. **Clone repository**
```bash
git clone https://github.com/your-username/laravel-blog.git
cd laravel-blog
