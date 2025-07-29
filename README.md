# Graphics Quiz Site - Neural Networks & Computer Graphics Quiz Platform

A web-based interactive quiz platform for testing knowledge in neural networks and computer graphics concepts with Hebrew language support.

## 📁 Repository Structure

```
├── index.html              # Main quiz application
├── schemas/                 # Schema and prompt files
│   ├── quiz-schema.json     # JSON schema for quiz questions
│   └── gemini_prompt.md     # AI prompt template for generating quizzes
├── questions/               # Quiz question files
│   └── questionsX.json      # Quiz files (numbered sequentially)
└── README.md               # This file
```

## 🎮 How to Use

Open `index.html` in any modern web browser. The application will automatically detect available quiz files and allow you to select which ones to use.

## 📝 Creating New Quiz Files

### Using AI Generation (Recommended)

1. **Prepare your content**: Gather lecture material or topic summary
2. **Use the prompt template**: Edit `schemas/gemini_prompt.md` with your content
3. **Generate**: Submit to AI tools (Gemini, ChatGPT, Claude, etc.)
4. **Validate**: Check output follows the schema in `schemas/quiz-schema.json`
5. **Save**: Save as `questions/questionsX.json` (where X is the next number)

### Schema Validation

To validate your quiz files against the JSON schema, you can use tools like:

- **AJV CLI**: `npm install -g ajv-cli` then `ajv validate -s schemas/quiz-schema.json -d questions/questionsX.json`
- **Online validators**: JSON Schema validators that accept custom schemas

### Manual Creation

Follow the JSON schema structure in `schemas/quiz-schema.json`. The schema supports:

- Multiple choice questions with 4 options
- Open-ended text questions
- Hebrew language content
- Detailed explanations for answers

### Integration

New quiz files are automatically detected by the application - no code changes needed. Just save your file in the `questions/` folder with the correct naming pattern.

---

**Happy Quiz Creating! 🎓**
