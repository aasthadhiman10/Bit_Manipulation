# 🕹️ Java Bit Manipulation Deep Dive

Welcome to the **Bit Manipulation** section of my Java Data Structures & Algorithms learning journey! This module focuses on low-level binary bit operations and bitmasking techniques.

---

## 🎯 Code Implementations

| File | Goal | Core Formula |
| :--- | :--- | :--- |
| **`Get_Bit.java`** | Find if bit at position `pos` is `0` or `1` | `(1 << pos) & n` |
| **`Set_Bit.java`** | Change bit at position `pos` to `1` | `(1 << pos) | n` |
| **`Clear_Bit.java`** | Change bit at position `pos` to `0` | `~(1 << pos) & n` |
| **`Update_Bit.java`** | Dynamically **Set** (`1`) or **Clear** (`0`) a bit | Conditional (`Set` / `Clear`) |

---

## 💡 How The Logic Works

### 🔍 1. Get Bit
Checks whether the bit at position `pos` is set (`1`) or unset (`0`).
```java
int bitMask = 1 << pos;
if ((bitMask & n) == 0) {
    System.out.println("Bit was zero");
} else {
    System.out.println("Bit was one");
}