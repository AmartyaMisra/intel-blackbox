# Google Dorking: Espionage for Civilians

*"Google isn't a search engine. It's an access terminal to unsecured data archives."*

Most people use Google to search *for* things.  
A few use Google to search *through* things.  
This is where civilian-grade espionage begins.

---

## 🧠 What is Google Dorking?

Google Dorking (or Google hacking) is the art of using advanced search operators to find sensitive information that's publicly available — but not meant to be found.

You’re not “hacking” in the illegal sense. You're just **asking better questions** than most people know how to ask.

> Think of it as digital lockpicking with a magnifying glass and surgical syntax.

---

## 🔍 Key Operators to Know

| Operator       | What It Does                              | Example                          |
|----------------|--------------------------------------------|----------------------------------|
| `site:`        | Limits search to a specific domain         | `site:gov.in filetype:xls`       |
| `filetype:`    | Finds specific file formats                | `filetype:pdf confidential`      |
| `inurl:`       | Searches keywords in URLs                  | `inurl:admin login`              |
| `intitle:`     | Searches keywords in page titles           | `intitle:index of password`      |
| `cache:`       | Shows Google's cached version of a page    | `cache:example.com`              |

---

## 🛠️ Real-World Dorking Examples

### 📁 1. Exposed Admin Panels
```bash
intitle:"admin panel" inurl:admin
