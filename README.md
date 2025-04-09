<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
</head>
<body>
    <h1>🧪 Protocol Design Agent</h1>
    <p>This tool helps generate the <strong>Introduction</strong> section of a <strong>clinical trial protocol</strong> based on study and drug metadata using LangChain and OpenAI's GPT model.</p>
    <div class="section">
    </div>
    <div class="section">
        <h2>🔧 Setup Instructions</h2>
        <h3>1. Clone the Repository</h3>
        <pre><code>git clone https://github.com/your-username/protocol-design-agent.git
cd protocol-design-agent</code></pre>
        <h3>2. Create Python Virtual Environment</h3>
        <pre><code>python -m venv venv
source venv/bin/activate   # On Windows use: venv\Scripts\activate</code></pre>
        <h3>3. Install Dependencies</h3>
        <pre><code>pip install -r requirements.txt</code></pre>
        <p><strong>requirements.txt</strong> should include:</p>
        <pre><code>pandas
python-dotenv
openai
langchain
langchain-community</code></pre>
        <h3>4. Add Your OpenAI API Key</h3>
        <p>Create a <code>.env</code> file and add:</p>
        <pre><code>API_KEY=your-openai-api-key-here</code></pre>
        <p><strong>Important:</strong> Never share your .env file publicly.</p>
    </div>
    <div class="section">
        <h2>🚀 How to Run</h2>
        <h3>1. Update Input File Path</h3>
        <pre><code>input_data = "your input file"</code></pre>
        <h3>2. Run the Agent</h3>
        <pre><code>run main.ipynb</code></pre>
        <p>The agent will read metadata, format it into a prompt, and ask GPT to generate the protocol introduction.</p>
    </div>
    <div class="section">
        <h2>📌 Output</h2>
        <p>If file access works, you'll get a generated introduction. If not, it will prompt you to manually provide metadata.</p>
    </div>
    <div class="section">
        <h2>🧠 Agent Details</h2>
        <ul>
            <li><strong>Model:</strong> gpt-4o-mini</li>
            <li><strong>Temperature:</strong> 0.1</li>
            <li><strong>Tool:</strong> ProtocolDesign</li>
            <li><strong>Framework:</strong> LangChain using Structured Chat agent</li>
        </ul>
    </div>
    <div class="section">
        <h2>🛠️ Troubleshooting</h2>
        <ul>
            <li><strong>File Not Found?</strong> Double-check the file path.</li>
            <li><strong>API Key Issue?</strong> Ensure your .env is set up and correctly loaded.</li>
            <li><strong>File Access?</strong> You might need to paste the metadata directly if file access fails.</li>
        </ul>
    </div>
    <div class="section">
        <h2>📤 Example Prompt Format</h2>
        <pre>
Metadata Input:
*** Study and Drug Metadata ***

Corresponding Introduction Section:
*** GPT-generated intro here ***
        </pre>
    </div>
    <div class="section">
        <h2>📬 Contact</h2>
    <p>Author: Gajulapalli Naga Vyshnavi<br>
    Contact: <a href="mailto:nvyshnavi36@gmail.com">nvyshnavi36@gmail.com </a><br>
    For any inquiries, feel free to reach out via the contact information provided.</p>
    </div>
</body>
</html>
