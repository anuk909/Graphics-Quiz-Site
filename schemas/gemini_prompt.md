# Quiz Generation Prompt for Neural Networks & Computer Graphics

## Context

You are creating a quiz for a computer graphics course focused on neural networks applications.

## Instructions

Create a quiz based on the lecture content provided in the PDF/DOCX file. Follow these guidelines:

1. **Question Types**: Mix of multiple choice and open-ended questions
2. **Language**: All content in Hebrew
3. **Format**: Must follow the JSON schema provided in the quiz-schema.json file exactly

## Output Requirements

- Valid JSON array following the schema
- Questions in Hebrew language, use English terms if it's relevant in the context
- 20 multiple choice and 10 open-ended questions
- Don't use the examples from the schema
- Don't use citing in the output file
- Clear, unambiguous questions
- Detailed explanations for all answers
- Solvable questions, not trivial or impossible
- Realistic distractors for multiple choice questions
