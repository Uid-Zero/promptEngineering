# Zero Shot [Basic] Prompting Framework

## Overview
Basic prompting refers to the simplest way of interacting with **LLMs** by providing direct instructions or queries. It is the foundation of prompt engineering and serves as the starting point for refining AI responses. 

## Best Practices for Basic Prompting
- **Be Clear and Specific**: Clearly define what you want from the model. 
- **Use Proper Grammar and Punctuation**: Helps the model better understand your intent.
- **Avoid Ambiguity**: Ensure that the query does not have multiple interpretations.
- **Provide Context When Necessary**: Helps the model generate more relevant responses.
- **Use Constraints If Needed**: Limit response length or specify the format [Give a one-paragraph summary].

## Examples

### Simple Query
```
Q: What is the capital of France? 
A: The capital of France is Paris.
```

### Instruction-Based Prompt
```
Q: Explain the theory of relativity in simple terms.
A: The theory of relativity, developed by Albert Einstein, explains how space and time are linked for objects moving at a constant speed. It has two main parts: Special Relativity [which deals with how time and space change at high speeds] and General Relativity [which explains how gravity affects time and space].
```

### Vague Query
> Q: Tell me something.

#### Issue:
- Too vague; does not specify what kind of information is needed.
- The response may be irrelevant to what the user expects.

### Ambiguous Request
> Q: How does it work?

#### Issue:
- ***It*** is unclear; the model has no context about what ***it*** refers to.

### Poorly Structured Prompt
> Q: explain relativity??

#### Issue:
- Lack of capitalization and punctuation makes the prompt harder to interpret.
- No indication of preferred response format or level of detail.

## Limitations of Zero Shot [Basic] Prompting
- **Lack of Context**: Basic prompts may generate generic or vague responses.
- **Short Responses**: Without additional instructions, responses might be too brief.
- **Difficulty Handling Complex Tasks**: For multi-step reasoning or problem-solving, basic prompts might not be enough.

## Improving Basic Prompts
- **Add Examples**: Provide context by showing desired outputs.
- **Use Directives**: Ask the model to ***explain step-by-step*** or ***list in bullet points***.
- **Specify Format**: Indicate whether you want a summary, table, JSON, or another format.