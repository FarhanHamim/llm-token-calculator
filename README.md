# LLM Token Calculator 📊
A web-based calculator for estimating token usage and costs across various large language models (LLMs).

# Features ✨
- Support for 15+ LLMs (GPT, Claude, Gemini, Llama, Mistral, DeepSeek)
- Real-time token calculation
- Cost estimation in USD
- Model-specific pricing presets
- Dark mode UI with gradient accents
- Responsive design
- Token preview while typing

# Live Demo 🌐
[!]
https://llm-token-calculator-new.vercel.app/

# Installation 💻
Prerequisites:
* Modern web browser
* GitHub account
* Basic understanding of HTML/JavaScript

# Local Setup

1. Clone the repository:

```
git clone https://github.com/your-username/llm-token-calculator.git
cd llm-token-calculator
```

2. Launch local server:

```
# Using Python
python -m http.server 8000

# Or using Node.js
npx serve
```

3. Open in browser:

```
http://localhost:8000
```

# Deployment 🚀
GitHub Pages:
i. Go to repository Settings > Pages
ii. Select branch main and folder / (root)
iii. Save - Your site will be at:

```
https://<your-github-username>.github.io/<repository-name>/
```

# Alternative Hosting
### Vercel:
Drag-and-drop the folder
### Netlify:
Continuous deployment from GitHub
### Cloudflare Pages:
Free edge hosting

# Usage Guide 📖
## Basic Usage
1. Select model from dropdown
2. Enter input/prompt text
3. Enter output/response text
4. View real-time token counts
5. See cost estimation below

## Advanced Features
* Custom Pricing: Override default prices
* Model Comparison: Switch models to compare costs
* Mobile Support: Works on all devices

# Customization 🎨
## Color Scheme
Modify CSS variables in :root:
```
:root {
    --primary: #6366f1;    /* Main brand color */
    --secondary: #4f46e5;  /* Secondary color */
    --bg: #0f172a;         /* Background color */
    --surface: #1e293b;    /* Card background */
    --text: #f8fafc;       /* Primary text */
}
```
# Adding Models
1. Update MODEL_INFO in JavaScript:
```
const MODEL_INFO = {
    'new-model': { 
        input: 0.000001, 
        output: 0.000002 
    }
};
```
2. Add to HTML dropdown:
```
<optgroup label="New Provider">
    <option value="new-model">Model Name</option>
</optgroup>
```

# Supported Models 🤖
| Provider | Models | 
| :---- | :----: |
| OpenAI | GPT-3.5 Turbo, GPT-4, GPT-4 Turbo |
| Anthropic | Claude 3 Opus, Claude 3 Sonnet |
| Google | Gemini Pro |
| Meta | Llama 2 70B, Llama 3 70B |
| Mistral |	Mistral 7B, Mixtral 8x7B |
| DeepSeek | DeepSeek Chat, MoE-16B, 67B |

# Contributing 🤝
1. Fork the repository
2. Create feature branch:
```
git checkout -b feature/new-feature
```
3. Commit changes:
```
git commit -m 'Add some feature'
```
4. Push to branch:
```
git push origin feature/new-feature
```
5. Open a Pull Request

# Acknowledgements 🙏
* GPT Tokenizer: gpt-tokenizer library
* Color Scheme: Inspired by Dracula Pro
* UI Design: Modern Web Practices

> [!NOTE]
> Always verify actual model pricing and tokenization methods with official provider documentation. Token counts may vary slightly between implementations.

