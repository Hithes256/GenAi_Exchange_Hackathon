# GenAi_Exchange_Hackathon

Steps to Execute 

1. Install required libraries
* Open your Jupyter Notebook / Colab / terminal and run:
pip install google-api-python-client google-auth-httplib2 google-auth-oauthlib        transformers torch gradio
2. Enable Google Docs API
1. Go to Google Cloud Console.
2. Create a new project (any name, like "Legal Analyzer").
3. In the search bar ? type Google Docs API ? Enable it.
4. Then go to APIs & Services ? Credentials.
5. Click Create Credentials ? OAuth Client ID.
6. Choose Desktop App.
7. Download the file ? it will be called credentials.json.
8. Put this file in the same folder as your Python script / Notebook.
3. First-time Authentication
* Run your script.
* A browser window will open asking you to log in with your Google account.
* Allow access ? it will create a file token.pkl in your folder.
* Next time, it won’t ask again (it will use token.pkl).
4. Prepare Your Google Doc
1. Open your legal document (PDF, Word, etc.) in Google Drive.
2. Right-click ? Open with ? Google Docs (this converts it to Google Docs format).
3. Copy the Document ID from the URL.
o Example:
o https://docs.google.com/document/d/1j9Iq644BOmpzUibxBIFxmV2fif4vGk8NXi0SCjfdfeg/edit
o Here, the Doc ID is: 1j9Iq644BOmpzUibxBIFxmV2fif4vGk8NXi0SCjfdfeg
5. Run Your Script
* Just run your full script (the one you pasted).
* Gradio will launch a small web app in your browser.
* If using Colab / Jupyter, it will show a shareable link.
6. Use the Web App
* Enter your Google Doc ID in the textbox.
* Optionally type a question (e.g., "What are the penalties for late payment?").
* Click Analyze Document.
* It will show:
o Summary
o Risky Clauses (with keywords like penalty, fine, termination)
o Amounts/Percentages mentioned
o Answer to your question

