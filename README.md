# 🇮🇳 TaxSetu – AI GST Compliance Platform

**TaxSetu** is an AI-powered GST compliance platform designed to simplify invoice processing, GST calculations, and compliance verification for businesses. It uses multiple AI agents to automate repetitive GST workflows, identify potential risks, and provide easy-to-understand explanations, including in Hindi.

## 🚀 Key Features

- **AI-Powered Invoice Processing:** Extracts relevant information from invoices using Gemini Vision.
- **Automated GST Calculations:** Helps calculate applicable GST amounts based on invoice details.
- **GST Filing Validation:** Checks filing-related information for potential inconsistencies.
- **GSTIN Validation:** Supports verification of GST identification details.
- **Input Tax Credit (ITC) Reconciliation:** Helps identify discrepancies in ITC-related records.
- **AI Risk Analysis:** Identifies potential compliance risks for further review.
- **Hindi Explanations:** Makes GST-related information easier to understand through AI-generated Hindi explanations.
- **Multi-Agent Architecture:** Uses five specialized AI agents for invoice processing, GST calculations, filing validation, risk analysis, and explanations.
- **Traceable AI Decisions:** Provides decision details to help users understand the system's outputs.

> **Note:** TaxSetu is an assistance tool. AI-generated results should be reviewed against official GST records and applicable regulations before making filing or financial decisions.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| React | Frontend user interface |
| Node.js | Backend runtime |
| Gemini API | AI-powered analysis and invoice extraction |
| Firebase | Application services and data management |
| Firebase Cloud Functions | Backend cloud functions |

## 🏗️ System Architecture

```text
              ┌──────────────────────┐
              │       React UI       │
              │  User & Invoice Data │
              └──────────┬───────────┘
                         │
                         ▼
              ┌──────────────────────┐
              │    Node.js Backend   │
              │  Request Processing  │
              └──────────┬───────────┘
                         │
                         ▼
              ┌──────────────────────┐
              │  AI Agent Coordinator│
              └──────────┬───────────┘
                         │
        ┌────────────────┼────────────────┐
        ▼                ▼                ▼
 ┌─────────────┐  ┌─────────────┐  ┌─────────────┐
 │   Invoice   │  │ GST & Filing│  │ Risk Analysis│
 │  Processing │  │ Validation  │  │    Agent    │
 └─────────────┘  └─────────────┘  └─────────────┘
                         │
                         ▼
              ┌──────────────────────┐
              │ ITC Reconciliation & │
              │ Hindi Explanation    │
              └──────────┬───────────┘
                         │
                         ▼
              ┌──────────────────────┐
              │ Results & Explanations│
              └──────────────────────┘
```

*Architecture shown is a conceptual overview; adapt it to match the actual implementation.*

## ⚙️ Getting Started

### Prerequisites

Install the following tools before running the project:

- Node.js and npm
- Git
- A Gemini API key
- A Firebase project configured for the services used by the application

### 1. Clone the Repository

```bash
git clone https://github.com/NP0149/taxset.git
cd taxset
```

### 2. Install Dependencies

If the project uses a single `package.json` at the root:

```bash
npm install
```

If the frontend and backend have separate `package.json` files, install dependencies in each directory:

```bash
cd frontend
npm install
cd ../backend
npm install
```

Replace `frontend` and `backend` with your actual directory names if they differ.

### 3. Configure Environment Variables

Create the appropriate `.env` file for your project and add the required configuration.

Example:

```env
GEMINI_API_KEY=your_gemini_api_key
```

Add Firebase configuration and other required variables according to your implementation.

**Security:** Never commit API keys, service-account credentials, or private configuration files to GitHub. Add `.env` to `.gitignore`.

### 4. Run the Application

Use the commands defined in your project's `package.json` files.

For example, if your root project defines a development script:

```bash
npm run dev
```

For a separate frontend and backend, start each using its configured development command.

## 🔄 How It Works

1. **Upload an invoice:** The user provides an invoice for processing.
2. **Extract information:** Gemini Vision helps extract relevant invoice fields.
3. **Process GST information:** The platform calculates GST and checks relevant GSTIN and filing details.
4. **Analyze compliance risks:** Specialized AI agents evaluate potential inconsistencies and risks.
5. **Reconcile ITC:** The system helps compare relevant input tax credit records.
6. **Generate explanations:** Users receive results and AI-generated explanations, including Hindi-language assistance.

## 🎯 Use Cases

- Small businesses managing GST invoices
- Finance teams reviewing invoice information
- Businesses checking GST calculations
- Preliminary ITC reconciliation
- Identifying potential GST compliance discrepancies
- Understanding GST-related information in Hindi

## 🔐 Security & Reliability

- Keep API keys and Firebase credentials private.
- Validate uploaded files and user inputs.
- Apply appropriate authentication and authorization.
- Review AI-generated results before relying on them.
- Use official GST records and applicable regulations for final verification.

## 🔮 Future Enhancements

- Integration with additional accounting systems
- Improved invoice validation and error reporting
- Enhanced compliance dashboards and analytics
- Support for additional Indian languages
- More comprehensive audit logs and reporting
- Integration with authorized GST data sources where available

## 👩‍💻 Author

**Navya Pasunuri**

- GitHub: [NP0149](https://github.com/NP0149)
- LinkedIn: [Navya Pasunuri](https://www.linkedin.com/in/navya-pasunuri-773a1b309/)

## 📄 License

Choose a license before distributing the project publicly. If you intend to use the MIT License, add a `LICENSE` file containing its terms.

---

**TaxSetu — Simplifying GST compliance with AI.**
