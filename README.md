# 🚀 termc

A tiny Python library that makes terminal apps look way cooler with almost no effort.

No more boring `print()` spam.
No more ugly CLI menus.
Just clean banners, colorful messages, menus, separators, and stylish prompts.

---

## 📦 Installation

```bash
pip install termc
```

Or clone the repository:

```bash
git clone https://github.com/waasaty/termc.git
```

---

## 🚀 Quick Start

```python
import termc

termc.Config.program_name("MyCoolApp")

termc.print_header()

termc.print_info("Application started")
termc.print_succes("Everything works!")
termc.print_warn("Something looks suspicious...")
termc.print_error("Oops, an error occurred")
termc.print_dbg("Debug message")
```

Output:

```text
╭─────────────╮
│ MyCoolApp   │
╰─────────────╯

[i] information
[✓] succes
[!] warning
[✗] error
[~] debug
```

---

## 📝 User Input

Create nice-looking input prompts:

```python
import termc

termc.input_start_header()

name = termc.input_middle("Enter your name")
age = termc.input_bottom("Enter your age")
```

Example:

```text
╭─ waasaty@MyCoolApp [12:12:12]
├─❯ Enter your name:
╰─❯ Enter your age:
```

---

## 📋 Menus

```python
termc.print_menu(
    "Main Menu",
    [
        "Start",
        "Settings",
        "Exit"
    ]
)
```

Output:

```text
╭───────────────╮
│ Main Menu     │
├───────────────┤
│ 1. Start      │
│ 2. Settings   │
│ 3. Exit       │
╰───────────────╯
```

---

## 🎨 Banners

```python
termc.print_banner("""
Welcome to
My Awesome App
""")
```

---

## 🔧 Configuration

Change the displayed program name:

```python
termc.Config.program_name("SuperApp")
```

Now prompts and headers will use:

```text
username@SuperApp
```

---

## 💡 Why termc?

Because writing:

```python
print("[INFO] Application started")
```

for the 500th time gets boring.

termc gives your terminal projects a cleaner and more professional look while keeping everything simple.

---

## 🤝 Contributing

Found a bug?
Have an idea?
Open an issue or submit a pull request.

Contributions are always welcome.

---

## 📜 License

MIT License

---
Do whatever you want, just don't claim you wrote it 😄