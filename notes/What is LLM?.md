<!-- slide template="[[tpl-llm]]" -->
<style>
  .side-image {
    transform: translateY(-1px);
  }
</style>

<split even gap="1">
  ![[openai_image_20250702_155831.png]]<!-- element class="side-image" style="height: 100%; width: 250px" -->

  <div style="display: flex; justify-content: center; align-items: center; height: 100%;">
    <div>
      <p class="text-xl q">What is LLM?</p>
      <p><strong>LLM or Large Language Model</strong> is specific Generative AI focus on text generation. LLM is a AI system trained on <strong>massive text dataset</strong> to understand and generate human-like text.<p>
    </div>
  </div>
</split>

---

<!-- slide template="[[tpl-llm]]" -->
<style>
code {
  font-size: 14px !important;
}
pre {
  font-size: 14px !important;
  color: #e2e8f0 !important;
}
</style>

<grid drag="48 65" drop="2 15">
![[Transformer.png]]
Source: [Attention is All you Need](https://proceedings.neurips.cc/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf)
</grid>

<grid drag="48 65" drop="50 15">
How it works?<!-- element class="text-xl q" style="padding-bottom:0" -->

```markdown
Text: "The cat sat"
    ↓
[Tokenize] → ["The", "cat", "sat"]
    ↓
[Embed] → [1.2, 0.8, 0.5] (convert to numbers)
    ↓
[Attention] → "Which words matter most?"
    ↓
[Transform] → Context-aware representations
    ↓
[Predict] → Next word: "on" (70% probability)
```
</grid>

note:
Frontier model like Claude or GPT-4 are trained on 10+ TB training data

---

<!-- slide template="[[tpl-llm]]" -->
### Terminology

---

<!-- slide template="[[tpl-llm]]" -->
<style>
li {
  font-size: 2rem;
}
</style>
<ul style="line-height: 2;">
	<li><strong>Tokenization</strong>  -> Breaking text into smaller units (tokens) that the model can process. Example: "ChatGPT is amazing!" → [Chat, G, PT, is, amaz, ing, !]</li>
	<li class="fragment" data-fragment-index="1"><strong>Prompt</strong> -> The input text/instructions you give to the LLM to get a desired output. Example prompt: "Summarize this article in 3 bullet points"</li>
	<li class="fragment" data-fragment-index="2"><strong>Inference</strong> -> The process of running the model to generate predictions/outputs.
	<li class="fragment" data-fragment-index="3"><strong>Zero-shot Learning</strong> -> Model performs a task without any examples in the prompt.
	<li class="fragment" data-fragment-index="4"><strong>Few-shot Learning</strong> -> Model learns from a few examples provided in the prompt.
</ul>

note:
- There are 5 important terminology you have to understand
- Training vs Inference: Training builds the model, inference uses it.
- The zero-shot and few-shot are belong to prompt engineering, there are a lot more terminology in Prompt Engineering

---

<!-- slide template="[[tpl-llm]]" -->
### Models

---

<!-- slide template="[[tpl-llm]]" -->
#### HuggingFace.co<!-- element style="margin:0"-->
The bigest open-source models repository and one of AI hosting platform.

![[2025-06-02-hugging-face.png]]<!-- element style="height:60%; margin:0" -->

---

<!-- slide template="[[tpl-llm]]" -->
#### OpenRouter.ai<!-- element style="margin:0"-->
LLM provider and router.

![[2025-06-02-openrouter.png]]<!-- element style="height:60%; margin:0" -->