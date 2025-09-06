## 📄 Document Parser AI

Python scripts to **parse, extract, and structure data from documents (PDFs, invoices, receipts, reports, etc.)**  
using **AI APIs** like [OpenAI](https://openai.com), [Anthropic](https://www.anthropic.com/), and [Invofox](https://invofox.ai/).

---

## 🚀 Features

- Extract text and structured data from **PDF documents**
- Support for **invoices, receipts, and general reports**
- Integration with **OpenAI, Anthropic, and Invofox APIs**
- Easy to extend for new document types
- Saves structured data into **JSON / CSV / Database**

---

## 🛠️ Tech Stack

- **Python 3.9+**
- `PyPDF2`, `pdfplumber`
- `openai`, `anthropic`
- `requests`
- `pandas`
- `invofox-sdk` (if applicable)

---

## 📊 Example Output

```
{
  "invoice_number": "INV-12345",
  "date": "2025-09-01",
  "total": "1500.00",
  "items": [
    {"description": "Product A", "qty": 2, "price": 500},
    {"description": "Product B", "qty": 1, "price": 500}
  ]
}
```

---

## What’s Inside

- Extract text from invoice PDFs with [pdfplumber](https://github.com/jsvine/pdfplumber)
- Parse invoice contents using:
  - OpenAI GPT-4 (`openai-main.py`)
  - Anthropic Claude (`anthropic-main.py`)
  - Invofox API (`invofox-main.py`)
- Includes sample invoice files (`invoice_sample.pdf`, `invoice_sample.jpg`)

---

## Prerequisites

- Python 3.8 or higher
- A virtual environment (Recommended)
- API keys for:
  - OpenAI (`OPENAI_API_KEY`)
  - Anthropic (`ANTHROPIC_API_KEY`)
  - Invofox (`INVOFOX_API_KEY`)

---

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/ramesh-852000/document-parser-ai.git
   cd document-parser-ai
   ```

2. Create and activate a virtual environment:

   ```bash
   python -m venv env
   source env/bin/activate    # macOS/Linux
   env\Scripts\activate     # Windows
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Create a `.env` file in the project root and add your API keys:

   ```env
   OPENAI_API_KEY=your-openai-api-key
   ANTHROPIC_API_KEY=your-anthropic-api-key
   INVOFOX_API_KEY=your-invofox-api-key
   ```

---

## Usage

- **OpenAI GPT-4**:

  ```bash
  python openai-main.py
  ```

- **Anthropic Claude**:

  ```bash
  python anthropic-main.py
  ```

- **Invofox API**:
  ```bash
  python invofox-main.py
  ```

---

Thanks for visiting!

## 📸 Preview

![Preview](samples/invoice_sample.jpg)
