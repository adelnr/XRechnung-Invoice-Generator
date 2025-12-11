# XRechnung-Invoice-Generator
A robust, lightweight WordPress plugin designed to generate dynamic, print-ready PDF invoices. The plugin includes a frontend invoice generator with real-time calculations, a flexible backend settings panel, and optimized A4 PDF rendering using DomPDF.

---

## 🚀 Features

### 🔹 Frontend Invoice Generator
- **Dynamic Line Items:** Add or remove invoice rows instantly.
- **Real-time Calculations:** Automatic calculation of totals, subtotals, VAT, and grand total via jQuery.
- **Responsive Design:** Fully styled, mobile-friendly invoice form (`.xr-invoice-form-container`).
- **Input Validation:** Required and numeric field validation built in.

### 🔹 Backend Configuration
- **Custom Column Management:** Admin can define invoice item columns (Key, Title, Required).
- **Branding Options:**
  - Upload Company Logo
  - Upload Digital Signature
- **Instant Previews:** Media uploads show immediate previews inside the settings panel.

### 🔹 PDF Generation
- **DomPDF Optimized Styles:** Uses `@page`, custom flex utilities, and A4 print rules.
- **A4 Layout:** 0.5cm margins, structured invoice layout.
- **High-Quality Typography:** Uses DejaVu Sans for UTF-8 compatibility.

---

## 🛠 Installation

1. Upload the plugin folder to `/wp-content/plugins/`.
2. Activate **XR Invoice Manager** from the WordPress *Plugins* page.
3. Go to **XR Settings** to configure VAT, currency, columns, and branding.

---

## ⚙️ Configuration

### 🔹 Global Settings
- **VAT Rate:** Set default tax percentage.
- **Currency Code:** Example: EUR, USD, AED.

### 🔹 Branding
- Upload **Company Logo** for invoice header.
- Upload **Signature Image** for footer signing.

### 🔹 Invoice Columns
1. Click **Add Column**
2. Set:
   - **Key** (e.g., `item_sku`)
   - **Title** (e.g., “SKU”)
   - **Required** checkbox
3. Plugin automatically handles quantity + price logic.

---

## 💻 Technical Details

### 🔹 File Structure
- **CSS Files**
  - Admin settings
  - Frontend form styles
  - Print/PDF styles (DomPDF)
- **JavaScript**
  - jQuery calculation engine
  - Media uploader integration

### 🔹 Targeted CSS Classes
- `.xr-invoice-form-container` — main form wrapper  
- `.xr-item-row` — invoice line item row  
- `.invoice-wrapper` — PDF layout container  
- `.xr-settings-wrap` — admin settings wrapper  

### 🔹 Stored Options
- Column data saved using the `xrechnung_columns` option key.

---

## 📦 Dependencies

- **jQuery**  
- **WordPress Media API**  
- **DomPDF** (required on server for PDF generation)

---


## 📬 Support

For customization, enhancements, or additional features, contact the developer.

