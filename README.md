# ChatBot Project - Persian RAG System

## English Description

This project implements a sophisticated Retrieval-Augmented Generation (RAG) chatbot system designed to answer questions about Linux, open-source software, and related topics using Persian language documents.

### Features

- **Multi-Source Data Integration**: Combines data from PDFs, Wikipedia articles, web content, and HTML files
- **Advanced Text Processing**: Persian text correction and character normalization
- **Vector Database**: Uses ChromaDB with multilingual embeddings for efficient document retrieval
- **Language Model**: Integrates with Cohere's Command-R-Plus model for high-quality responses
- **Document Chunking**: Intelligent text splitting with overlap for better context preservation

### Key Components

1. **Data Sources**:
   - Persian PDF documents about Linux and open-source software
   - Wikipedia articles (Richard Stallman, Linus Torvalds, GNU Project, etc.)
   - Web content from Linux resources
   - HTML files from Stallman's website

2. **Text Processing**:
   - Persian character correction and normalization
   - Smart document splitting with context preservation
   - Multi-language text handling

3. **RAG Pipeline**:
   - Document embedding using `multilingual-e5-large` model
   - ChromaDB vector storage for fast similarity search
   - Context-aware question answering with Cohere LLM

### Technical Stack

- **LangChain**: Document processing and RAG pipeline
- **ChromaDB**: Vector database for document storage
- **HuggingFace Embeddings**: Multilingual text embeddings
- **Cohere API**: Language model for question answering
- **PyPDFium2**: PDF document processing

### Usage

The system is designed to answer questions about:
- Linux operating system and its history
- Open-source software development
- Key figures like Linus Torvalds and Richard Stallman
- GNU Project and Free Software Foundation
- Programming concepts and software engineering

---

## توضیحات فارسی

این پروژه یک سیستم چت‌بات پیشرفته مبتنی بر RAG (بازیابی-تقویت شده تولید) است که برای پاسخ به سوالات درباره لینوکس، نرم‌افزارهای متن‌باز و موضوعات مرتبط با استفاده از اسناد فارسی طراحی شده است.

### ویژگی‌ها

- **ادغام داده از منابع متعدد**: ترکیب داده‌ها از PDF، مقالات ویکی‌پدیا، محتوای وب و فایل‌های HTML
- **پردازش متن پیشرفته**: تصحیح متن فارسی و عادی‌سازی کاراکترها
- **پایگاه داده برداری**: استفاده از ChromaDB با embedding چندزبانه برای بازیابی کارآمد اسناد
- **مدل زبانی**: یکپارچگی با مدل Command-R-Plus شرکت Cohere برای پاسخ‌های با کیفیت
- **تکه‌بندی اسناد**: تقسیم هوشمند متن با همپوشانی برای حفظ بهتر زمینه

### اجزای کلیدی

۱. **منابع داده**:
   - اسناد PDF فارسی درباره لینوکس و نرم‌افزارهای متن‌باز
   - مقالات ویکی‌پدیا (ریچارد استالمن، لینوس توروالدز، پروژه گنو و غیره)
   - محتوای وب از منابع لینوکس
   - فایل‌های HTML از وب‌سایت استالمن

۲. **پردازش متن**:
   - تصحیح و عادی‌سازی کاراکترهای فارسی
   - تقسیم هوشمند اسناد با حفظ زمینه
   - پردازش متن چندزبانه

۳. **خط لوله RAG**:
   - embedding اسناد با استفاده از مدل `multilingual-e5-large`
   - ذخیره‌سازی برداری ChromaDB برای جستجوی سریع شباهت
   - پاسخ‌دهی آگاه از زمینه با LLM شرکت Cohere

### پشته فناوری

- **LangChain**: پردازش اسناد و خط لوله RAG
- **ChromaDB**: پایگاه داده برداری برای ذخیره‌سازی اسناد
- **HuggingFace Embeddings**: embedding متن چندزبانه
- **Cohere API**: مدل زبانی برای پاسخ به سوالات
- **PyPDFium2**: پردازش اسناد PDF

### کاربرد

این سیستم برای پاسخ به سوالات درباره موارد زیر طراحی شده است:
- سیستم‌عامل لینوکس و تاریخ آن
- توسعه نرم‌افزارهای متن‌باز
- شخصیت‌های کلیدی مانند لینوس توروالدز و ریچارد استالمن
- پروژه گنو و بنیاد نرم‌افزار آزاد
- مفاهیم برنامه‌نویسی و مهندسی نرم‌افزار

## Installation & Setup

```bash
# Install required packages
pip install langchain
pip install langchain-community
pip install langchain-huggingface
pip install langchain-cohere
pip install langchain-chroma
pip install wikipedia
pip install chromadb

# Set up Cohere API key
export COHERE_API_KEY="your_api_key_here"
```

## Project Structure

```
ChatBot_Project/
├── ChatBot_Project.ipynb    # Main notebook with RAG implementation
├── .gitignore              # Git ignore file
├── data/                   # Data directory
│   ├── justforfun_persian.pdf
│   └── html/              # HTML files from Stallman's website
└── chroma_db2/            # ChromaDB vector store
```

## Author

**Mohammad Sadegh Seifi**

## License

This project is for educational purposes.
