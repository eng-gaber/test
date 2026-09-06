# 📄 OCR Error Analysis Report (Qwen3-VL-8B)

> **Note:** All punctuation marks (`.`, `,`, `:`, `«`, `»`, `()`), diacritics, Alef Hamzas (`أ`/`إ`/`آ` $\rightarrow$ `ا`), and Ya/Alef Maqsura (`ي`/`ى` $\rightarrow$ `ي`) are **ignored** during evaluation.

---

## 📊 Executive Summary
- **Average Model Accuracy:** **`97.26%`**

| Document Name | Accuracy % | Missed Words | Extra Words | Substituted Words |
| :--- | :--- | :--- | :--- | :--- |
| `00000004.txt` | **91.79%** | 2 | 3 | 7 |
| `00000006.txt` | **97.55%** | 0 | 5 | 5 |
| `00000007.txt` | **98.89%** | 1 | 0 | 1 |
| `00000008.txt` | **98.68%** | 0 | 1 | 3 |
| `00000010.txt` | **99.39%** | 0 | 0 | 6 |

---

## 🖼️ Document: `00000004.txt`
- **Accuracy:** `91.79%`
- **Ground Truth Word Count:** `80` words
- **Model Output Word Count:** `81` words

### ❌ Missed Words (Present in Ground Truth, skipped by model):
```
الرحيم, ١٢
```

### ➕ Extra Words (Inserted / Hallucinated by model):
```
١٧, به, التوقيع
```

### 🔄 Substituted Words (Ground Truth Word ➡️ What Model Read):
| Ground Truth Word | Model Prediction |
| :--- | :--- |
| `بسم` | `بم` |
| `الله` | `سلطة` |
| `الرحمن` | `البحرين` |
| `العربي` | `المركزي` |
| `العربي` | `المركزي` |
| `والنظام` | `والتنظيم` |
| `الثاني` | `الاخر` |

---

## 🖼️ Document: `00000006.txt`
- **Accuracy:** `97.55%`
- **Ground Truth Word Count:** `58` words
- **Model Output Word Count:** `63` words

### ❌ Missed Words (Present in Ground Truth, skipped by model):
✅ *No words missed!*

### ➕ Extra Words (Inserted / Hallucinated by model):
```
ه, م, م, ه, م
```

### 🔄 Substituted Words (Ground Truth Word ➡️ What Model Read):
| Ground Truth Word | Model Prediction |
| :--- | :--- |
| `١٣٩٤ه` | `١٣٩٤` |
| `١٩٧٤م` | `١٩٧٤` |
| `١٩٨٨م` | `١٩٨٨` |
| `١٤٠٨ه` | `١٤٠٨` |
| `١٤٠٨ه` | `١٩٨٨` |

---

## 🖼️ Document: `00000007.txt`
- **Accuracy:** `98.89%`
- **Ground Truth Word Count:** `128` words
- **Model Output Word Count:** `127` words

### ❌ Missed Words (Present in Ground Truth, skipped by model):
```
الموقعة
```

### ➕ Extra Words (Inserted / Hallucinated by model):
✅ *No extra words inserted!*

### 🔄 Substituted Words (Ground Truth Word ➡️ What Model Read):
| Ground Truth Word | Model Prediction |
| :--- | :--- |
| `والمصالح` | `والمسالح` |

---

## 🖼️ Document: `00000008.txt`
- **Accuracy:** `98.68%`
- **Ground Truth Word Count:** `134` words
- **Model Output Word Count:** `135` words

### ❌ Missed Words (Present in Ground Truth, skipped by model):
✅ *No words missed!*

### ➕ Extra Words (Inserted / Hallucinated by model):
```
عربية
```

### 🔄 Substituted Words (Ground Truth Word ➡️ What Model Read):
| Ground Truth Word | Model Prediction |
| :--- | :--- |
| `ينشيء` | `ينشي` |
| `ولمباديء` | `ومبادي` |
| `الاتية` | `التالية` |

---

## 🖼️ Document: `00000010.txt`
- **Accuracy:** `99.39%`
- **Ground Truth Word Count:** `203` words
- **Model Output Word Count:** `203` words

### ❌ Missed Words (Present in Ground Truth, skipped by model):
✅ *No words missed!*

### ➕ Extra Words (Inserted / Hallucinated by model):
✅ *No extra words inserted!*

### 🔄 Substituted Words (Ground Truth Word ➡️ What Model Read):
| Ground Truth Word | Model Prediction |
| :--- | :--- |
| `٤٣` | `٤٢` |
| `الموافقين` | `المرافقين` |
| `للفقرتين` | `للفرقتين` |
| `والمتوسطة` | `والتوسطة` |
| `لاية` | `لاي` |
| `اية` | `اي` |

---
