# 🌐 UXML — User Experience Markup Language

**UXML** is a universal, human-readable **markup language for describing user interface layouts** across platforms.  
Inspired by the simplicity of **JSON**, the structure of **HTML**, and the clarity of **Mermaid**, UXML lets you define screens, components, and user flows — **without writing a line of imperative UI code**.

---

## ✨ Why UXML?

Modern UIs are fragmented across platforms, frameworks, and screen sizes. HTML is web-first. Figma is design-only. React Native, Flutter, SwiftUI — all have their own ways of thinking.

We believe:

- UI should be **platform-agnostic**
- Layout should be **declarative and shareable**
- Designers and developers should speak the **same structural language**

UXML provides a common syntax for describing **what a screen looks like**, not how it works — a single source of truth for layout.

---

## 🧠 What UXML Is

- ✅ A declarative, tree-based layout syntax  
- ✅ Human-readable, based on JSON-like structure  
- ✅ Platform-independent: describe once, render anywhere  
- ✅ Easy to convert into HTML, React, Flutter, or prototyping tools  
- ✅ Ideal for mockups, live UI previews, and AI-generated interfaces

---

## 🚫 What UXML Is Not

- ❌ A replacement for programming UI behavior  
- ❌ A new visual design tool  
- ❌ A one-size-fits-all frontend framework  
- ❌ Tied to any specific platform or language

---

## 🖥 Example: A Login Screen

```json
{
  "type": "Screen",
  "props": { "name": "Login" },
  "children": [
    {
      "type": "Column",
      "props": { "align": "center", "gap": 16 },
      "children": [
        { "type": "Text", "props": { "text": "Welcome Back", "fontSize": 24 } },
        { "type": "Input", "props": { "placeholder": "Email" } },
        { "type": "Input", "props": { "placeholder": "Password", "secure": true } },
        { "type": "Button", "props": { "text": "Sign In", "onClick": "loginUser" } }
      ]
    }
  ]
}
