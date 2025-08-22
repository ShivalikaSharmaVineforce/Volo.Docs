# Asset Management

Welcome to the **Asset Management Documentation**.  
This document explains the basic concepts and usage of the Asset Management module.

---

## 📖 Overview
The Asset Management module helps organizations keep track of their physical and digital assets.  
It provides functionality to register, categorize, allocate, and monitor assets within your system.

---

## 🏗 Features
- Asset registration (add new assets with details like name, type, purchase date, etc.)
- Asset categories (organize assets by type or purpose)
- Asset allocation (assign assets to employees, projects, or departments)
- Asset tracking (status: active, in repair, disposed, etc.)
- Reporting and audit logs

---

## 📂 Asset Entity Structure
Example fields you might have in your database:

| Field Name     | Type        | Description                                |
|----------------|------------|--------------------------------------------|
| **Id**         | Guid / Int | Unique identifier for the asset             |
| **Name**       | String     | Name of the asset (e.g., Laptop, Printer)  |
| **CategoryId** | Guid / Int | Foreign key to asset category               |
| **PurchaseDate** | DateTime | When the asset was purchased               |
| **Status**     | Enum       | Current status (Available, In Use, etc.)   |

---

## 🚀 Usage
### Adding a New Asset
1. Navigate to **Asset Management > Assets**.
2. Click on **New Asset**.
3. Enter details such as **Name**, **Category**, **Purchase Date**, and **Status**.
4. Save.

### Viewing Assets
- Go to **Assets List** to see all registered assets.
- Use filters (e.g., category, status) to narrow down results.

### Updating Asset Information
- Select an asset from the list.
- Click **Edit** and update details.
- Save changes.

---

## 🔗 Related Links
- [Asset Categories](categories.md)
- [Asset Allocation](allocation.md)
- [Audit Logs](audit.md)

---

📌 **Tip:** You can create multiple `.md` files like `categories.md`, `allocation.md`, `audit.md`, and link them together for a structured documentation experience in **VoloDocs**.
