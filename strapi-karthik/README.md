
# 🚀 Strapi CMS Setup - Articles API

This project sets up a Strapi CMS locally to manage and publish content using the `Article` collection type.

---

## 📦 Prerequisites

- Node.js
- npm or yarn
- Strapi (installed globally or via `npx`)
- MongoDB/PostgreSQL (optional for custom DB)

---

## 🛠️ Installation & Setup

1. **Create a Strapi Project:**

```bash
npx create-strapi-app@latest my-strapi-project --quickstart
````

2. **Start the Development Server:**

```bash
cd my-strapi-project
npm run develop
```

3. Open Strapi Admin Panel:

```
http://localhost:1337/admin
```

Register your admin account to proceed.

---

## 🧱 Create `Article` Collection Type

1. Go to **Content-Type Builder**

2. Create a new **Collection Type** named: `Article`

3. Add the following fields:

   * `title` (Text, required)
   * `content` (Rich Text (Blocks))
   * `boolean` (true or false)

4. Save the schema and allow Strapi to restart.

---

## 🧑‍🔧 Configure Public Permissions

1. Go to: `Settings > Roles > Public`
2. Under **Article**, enable:

   * `find`
   * `findOne`
3. Save the permissions

---

## 📝 Add and Publish Content

1. Go to **Content Manager > Articles**
2. Click **Create new entry**
3. Fill in the fields, and click **Publish**

---

## 🔍 Test the API

Use browser, Postman, or curl to test:

```bash
GET http://localhost:1337/api/articles
```

You should see your published content in JSON format.

---

## 📂 Project Structure (Key Parts)

```
my-strapi-project/
├── src/
│   └── api/
│       └── article/
│           ├── controllers/
│           │   └── article.js
│           ├── routes/
│           │   └── article.js
│           └── services/
│               └── article.js
```

---

## ✅ Notes

* API path is always plural (`/api/articles`) by default.
* Only **published entries** with proper **public permissions** will appear in API responses.

---

## 📬 Contact

> Maintained by **Karthik** – DevOps Intern 

