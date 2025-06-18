# n8n + SeaTable + Gotenberg PDF Generation

This repository contains example workflows and templates for generating dynamic PDFs using n8n, SeaTable, and Gotenberg.

## What's included

- **HTML Templates**: Invoice templates that demonstrate how to integrate dynamic data from SeaTable
- **n8n Workflows**: Complete workflow examples showing the progression from basic PDF generation to fully configurable templates
- **SeaTable Base**: SeaTable base template for PDF configuration

## How it works

The workflows demonstrate how to:
- Use SeaTable as a configuration backend for PDF templates
- Fetch logos, text, and formatted content from SeaTable
- Convert HTML templates with dynamic data into PDFs using Gotenberg
- Handle both simple text values and formatted rich text content

## Getting started

For a complete step-by-step tutorial, check out the blog post:
**[Generating Dynamic PDFs with Gotenberg, n8n, and SeaTable](https://cloudvox.at/a/generating-dynamic-pdf-with-gotenberg-n8n-and-seatable/)**

## Files structure

```
├── html/
│   ├── invoice.html                    # Basic static template
│   ├── invoice-with-logo.html         # Template with logo integration
│   ├── invoice-with-logo-email.html   # Template with logo and email
│   └── invoice-final.html             # Complete template with formatted text
├── seatable/
│   └── PDF Demo.dtable                 # SeaTable base template
└── workflows/
    ├── 01-PDF_Invoice_from_HTML.json  # Basic PDF generation
    ├── 02-PDF_Invoice_from_HTML.json  # With logo and email
    └── 03-PDF_Invoice_from_HTML.json  # Complete workflow
```

## Requirements

- n8n instance
- SeaTable account and API access
- Gotenberg service (demo available at https://demo.gotenberg.dev/)

## Note

These are example workflows designed to demonstrate functionality. For production use, you'll want to add proper error handling, optimize data fetching, and implement security best practices.
