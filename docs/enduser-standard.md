# Japanese End-User Software Standards

## Overview
Japanese end users at this manufacturing company often have specific expectations for how software screens and reports should look. These conventions are shaped by long-standing business practices, paper-based workflows, and local input methods.

---

## UI Standards for Numbers
- **Numeric alignment**: Amounts and values must be aligned to the **right side of the column**.  
- **Numeric formatting**: Numbers are expected in the format `xxx,xxx` (with comma separators), consistent with Japanese accounting and reporting practices.  
- **Negative numbers**: Often displayed with a preceding minus sign (`-123,456`) or enclosed in parentheses `(123,456)` depending on accounting standards.  
- **Decimal input**: Users expect precise decimal entry, especially for financial and manufacturing values. Input fields must support decimal places without rounding errors.  
- **Number field UX**: When a user clicks into a numeric input field, the default `0` must be removed and the field should appear **blank**, allowing the user to type freely without needing to delete the placeholder.  

---

## UI Standards for Dates
- **Formal Kanji format**: `YYYY年MM月DD日` (e.g., `2025年12月24日`), used in official documents and reports.  
- **Numeric format**: `YYYY/MM/DD` (e.g., `2025/12/24`), common in business systems and input fields.  
- **Era-based format (和暦)**: e.g., `令和7年12月24日`, sometimes used in government or traditional contexts.  

---

## 🔤 Typography Standards 
- **Font size preference**: Older end users often request larger text for readability. 
- **Recommended sizes**: 
    - Menu items → **28px** 
    - Titles/Headers → **24px** 
    - Normal text → **22px** 
- **Consistency**: Maintain uniform font sizes across screens to avoid confusion. 
- **Accessibility**: Consider adjustable font size settings for users with different

---

## General UX Conventions
- **Table-based layouts**: Data is expected in structured tables like Excel, not cards or dashboards.  
- **Compact design**: Minimal whitespace, dense information per screen.  
- **JP keyboard support**: Input fields must handle Japanese IME (Input Method Editor) correctly, including full-width/half-width characters, kana/kanji conversion, and proper handling of numeric entry alongside text.  
- **Scrolling behavior**: Users avoid **horizontal scrolling**. Screens should be designed for **vertical scrolling only**, with information flowing top-to-bottom.  

---

## 🕗 Pending UX Areas 
The following areas have not yet been requested or clarified by end users:
- Color preferences
- Button & action placement 
- Error messages 
- Search & filter behavior
- Export & Print 
- Security & session handling 

---

## Purpose
Documenting these conventions helps developers outside Japan understand why users request certain layouts or features, even if they seem unusual compared to Western UX practices.  

---

## Future Plan
To support engineers working with Japanese companies, I plan to build a **Japan UI/UX Standards Library** that:  
- Provides reusable components following these conventions.  
- Supports JP keyboard input, numeric formatting rules, and date formats.  
- Implements UX rules like vertical scrolling preference and blanking out default `0` in number fields.  
- Allows customization per project while keeping core standards intact.  
- Simplifies development by embedding cultural expectations into the design system.  
