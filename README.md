# 📋 JavaScript Forms & Validation

Practice tasks covering form handling, input validation, and regex in JavaScript.

---

## 🗂️ Tasks Overview

| # | Task | Topics |
|---|------|--------|
| 1 | Basic Form Handling | DOM access, prevent reload, display output |
| 2 | Basic Validation | Required fields, letters-only, error messages |
| 3 | Regex Validation | Email regex, phone number (10 digits) |
| 4 | Advanced Registration Form | Password rules, confirm fields, date validation |

---

## ✅ Task 1 — Basic Form Handling

**File:** `Task1_3.html`

A simple form that captures user input and displays it on the page without reloading.

**Fields:** First Name · Last Name · Email

**Key Concepts:**
- `event.preventDefault()` to stop page reload
- Accessing input values via `document.getElementById`
- Updating the DOM to display submitted data

---

## 🟡 Task 2 — Basic Validation

**File:** `Task1_3.html`

Validation layer added on top of Task 1.

**Rules:**
- All fields are required
- First & Last Name must contain letters only

**Key Concepts:**
- Inline error messages shown in red
- `.classList.add("invalid")` for red border styling
- Form blocked from submitting if any rule fails

---

## 🟠 Task 3 — Regex Validation

**File:** `Task1_3.html`

Upgraded validation using regular expressions.

**Added Field:** Phone Number

**Regex Patterns Used:**

```js
const emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
const phonePattern = /^\d{10}$/;
```

**Rules:**
- Email must follow a valid format
- Phone must be exactly 10 digits, numbers only

---

## 🔵 Task 4 — Advanced Registration Form

**File:** `RegistrationForm.html`

A full registration form with complex validation rules.

**Fields:** First Name · Last Name · Date of Birth · Email · Confirm Email · Password · Confirm Password

**Validation Rules:**

| Field | Rule |
|-------|------|
| Name | Letters only |
| Date of Birth | Required, must be a valid date |
| Email | Valid format via regex + must match Confirm Email |
| Password | Starts with capital letter, ≥2 digits, ≥1 special char, 8–32 chars |
| Confirm Password | Must match Password |

**Password Regex:**
```js
const passwordPattern = /^(?=[A-Z])(?=.*?\d.*?\d)(?=.*?[!@#$%^&*])(?=.{8,32}$)/;
```

**Features:**
- Error messages displayed under each invalid field
- All inputs highlighted in red on error
- Footer error message shown if any validation fails
- Success alert on valid submission

---

## 🛠️ Tech Stack

- HTML5
- CSS3
- Vanilla JavaScript

```bash
git clone https://github.com/h-othman1515/<repo-name>.git
```
