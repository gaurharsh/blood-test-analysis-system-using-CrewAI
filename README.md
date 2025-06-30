# 🧬 Blood Test Report Analyser (CrewAI)

## ✅ Bugs Fixed
- Refactored unrealistic task prompts
- Bound agents with correct tools
- Fixed `llm` initialization issue
- Made `read_data_tool()` async static method
- Awaited async methods properly
- Added missing imports and PDF support

## 🛠️ Setup Instructions

1. Clone the repo:
```
git clone https://github.com/your-username/blood-analyser.git
cd blood-analyser


2.  install dependencies:
```
 pip install -r requirements.txt


3. Set environment variables in .env:

    OPENAI_API_KEY=your-key
    SERPER_API_KEY=your-key

4. Run the server:
    uvicorn main:app --reload


🔍 API Usage:

 Endpoint: /analyze
 Method: POST

 Form Data:

 file: PDF file of blood report

 query: Optional query for insights


Returns  :
```
{
  "status": "success",
  "query": "Summarise my Blood Test Report",
  "analysis": "...",
  "file_processed": "blood_test_report_x.pdf"
}





