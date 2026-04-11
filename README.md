# Shopify Theme Technical Assignment – WPPOOL

## 👤 Candidate Info
Name: Hafiz Muhammad Ali
Email: hafiz.muhammadali.shehzad@gmail.com
Whatsapp Phone : +92-309-4992848  

---

## 📌 Project Overview

This project is a custom Shopify theme built on the Dawn theme as part of the WPPOOL technical assignment.

The goal was to implement advanced eCommerce functionality beyond Shopify’s native capabilities, focusing on dynamic product configuration, customer segmentation, and performance-friendly integrations.

---

## 🛠 Tech Stack

- Shopify (Dawn Theme)
- Liquid (Shopify Templating)
- JavaScript (Vanilla JS)
- HTML / CSS

---

## 🚀 Features Implemented

---

### 1️⃣ Multi-Step Product Configurator (PDP)

A fully custom product configurator was built to handle complex product options that cannot be managed using Shopify variants.

#### Key Features:

- Multi-step UI:
  - Model
  - Ventilation
  - Molding
  - Size Modification
  - Order Options

- Field Types:
  - Dropdowns
  - Text Input (Color Code)
  - Conditional Fields (e.g. Broan → CFM options)

- Conditional Logic:
  - Fields dynamically show/hide based on previous selections

- Dynamic Pricing:
  - Price updates live based on selected options

- Add to Cart:
  - All selections are passed as **line item properties**

- Cart Drawer:
  - Displays full configuration summary

> Note: Shopify’s base price is used in cart. Price adjustments are expected to be handled via Cart Transform Functions.

---

### Additional PDP Features

- Vimeo Video:
  - Displays only if product metafield is present

- Estimated Shipping:
  - Configurable via theme settings (Quick vs Standard)

- Unavailable State:
  - Configurator and Add-to-Cart hidden if product is unavailable

---

### 2️⃣ Customer Group-Based Collection Filtering

- Implemented using:
  - Customer tags (`wholesale`)
  - Product tags (`wholesale-only`)

#### Behavior:

- Wholesale customers → see all products
- Regular customers → cannot see wholesale-only products

> Implementation is handled in Liquid to completely exclude products from rendering.

---

### 3️⃣ Announcement Bar

- Supports multiple rotating messages
- Configurable via theme editor
- Auto-rotation speed control
- Dismiss functionality (per session using sessionStorage)
- Fully hides when all messages are dismissed

---

### 4️⃣ Live Chat Integration (Tawk.to)

- Integrated using script injection
- Non-blocking loading for performance
- Toggle ON/OFF via theme settings

---

### 5️⃣ Purchase Flow Verification

- Product successfully added to cart
- Checkout completed
- Order verified in Shopify admin

---

## 🎯 Design Decisions

- Used custom liquid blocks for flexible UI positioning
- Avoided Shopify variants due to scalability limitations
- Implemented line item properties for accurate data passing
- Focused on functionality over visual polish as per assignment instructions

---

## ⚠️ Limitations / Future Improvements

- Configurator is currently static (hardcoded options)
  - Can be improved using Shopify metafields for full dynamic control

- UI can be further enhanced for better user experience

- Expivi 3D integration not implemented (placeholder approach possible)

---

## 🔗 Setup Instructions

1. Create a Shopify Partner development store  
2. Install Dawn theme  
3. Upload theme files from this repository  
4. Assign theme as active  
5. Add sample products and required tags:
   - `wholesale-only`
   - Customer tag: `wholesale`

---

## 🎥 Walkthrough Video

https://www.loom.com/share/82efbe589a4143608eeb038d041b0457
---

## 📌 Submission Notes

- All core requirements have been implemented  
- Bonus task (Analytics Pixels) is completed  
- The focus was on logic, scalability, and Shopify best practices  

---

## 🙌 Thank You

Thank you for reviewing my submission!
