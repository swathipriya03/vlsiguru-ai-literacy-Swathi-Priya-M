# Week 01 Questions

## Q1 - AI → ML → Deep Learning → Generative AI → Agents

### A - Answer

Artificial Intelligence (AI) is the broad field of creating systems that can perform tasks that normally require human-like intelligence.

Machine Learning (ML) is a part of AI where systems learn patterns from data instead of relying only on explicitly programmed rules.

Deep Learning (DL) is a type of machine learning that uses multi-layer neural networks to learn complex patterns.

Generative AI refers to AI systems that can create new content such as text, images, audio, or code.

An AI agent is a system that can combine an AI model with tools and a workflow to perform actions toward a goal.

Simple relationship:

AI
└── Machine Learning
    └── Deep Learning

Generative AI can be built using machine-learning and deep-learning techniques.

An AI agent is better understood as a system or workflow that can use a model, tools, and actions rather than simply being another level in the hierarchy.

Examples:
- AI: a voice assistant
- ML: spam detection
- Deep Learning: image recognition
- Generative AI: an AI assistant generating an email
- AI Agent: a system that searches information and uses tools to complete a task

### E - Evidence

I checked these definitions against the Week 1 course material and reliable technical sources.

### V - Verification

I compared the definitions and checked that AI is the broad concept, ML is a learning-based approach, deep learning uses neural networks, generative AI creates content, and an agent can combine a model with tools and actions.

### R - Reflection

I learned that these terms are related but are not interchangeable. Generative AI focuses on creating content, while an agent is a larger system that can use models, tools, and workflows to accomplish a goal.


## Q2 - Is Everything That Looks Intelligent Actually AI?

### A - Answer

| Example | Classification | Reason |
|---|---|---|
| Calculator produces 25 × 16 = 400 | Traditional software | It follows explicit mathematical instructions. |
| If temperature > 80°C → WARNING | Traditional software | The rule was explicitly programmed. |
| Email identifies spam using learned patterns | Machine-learning AI | It uses patterns learned from previous data. |
| AI assistant summarizes a document | Generative AI | It generates new text based on the document. |
| Navigation app predicts arrival time | Machine-learning AI | It can use traffic and historical data to make predictions. |

A traditional program follows explicitly defined instructions. A machine-learning system can learn patterns from data and use them to make predictions or classifications.

### E - Evidence

I used the Week 1 material's distinction between traditional automation, machine-learning AI, and generative AI.

### V - Verification

I checked whether each example depended on explicitly programmed rules or on patterns learned from data or generated content.

### R - Reflection

I learned that something can appear intelligent without actually being AI. I should check how a system works instead of assuming that every automated feature is AI.


## Q3 - What Happens When You Ask an LLM a Question?

### A - Answer

When a user enters a question, the text becomes the prompt. The model processes the prompt as tokens and uses the available context to predict possible next tokens.

The model uses probabilities to select tokens and continues generating them until it produces a response.

Basic flow:

Prompt
→ Tokens
→ Model processing
→ Probability distribution
→ Next-token selection
→ Generated response

Training is the process where the model learns patterns from training data. Inference is when an already-trained model receives a prompt and generates a response.

### E - Evidence

The Week 1 guide gives the flow:

Prompt → Tokens → Model processing → Probability distribution → Next token selection → Generated response.

### V - Verification

I checked my explanation against a reliable technical or educational source and confirmed the basic process and the difference between training and inference.

### R - Reflection

I learned that an LLM generates a response through repeated next-token prediction. A fluent response does not automatically mean that every statement in it is true.


## Q4 - Hallucination Experiment

### A - Answer

I asked the same question to two AI assistants:

> What is the boiling point of pure water at standard atmospheric pressure, and what happens to the boiling point when atmospheric pressure decreases?

| Item | Gemini | Claude |
|---|---|---|
| Response summary | Gemini said that pure water boils at 100°C at 1 atm and that the boiling point decreases when atmospheric pressure decreases. | Claude gave the same main answer and also explained vapor pressure, altitude, vacuum conditions, and pressure cookers. |
| Main claim | Water boils at about 100°C at standard atmospheric pressure and its boiling point decreases when pressure decreases. | Water boils at about 100°C at 1 atm and its boiling point decreases when surrounding pressure decreases. |

### E - Evidence

I checked the important claims against an independent reliable reference about the boiling point of water and pressure.

Reference used:
https://webbook.nist.gov/cgi/cbook.cgi?ID=C7732185&Mask=224

The reference confirms that water boils at approximately 100°C at standard atmospheric pressure and that decreasing pressure lowers the boiling temperature.

### V - Verification

I compared the answers from Gemini and Claude with the independent reference.

Both AI assistants agreed on the main claims, and I did not find an obvious contradiction with the reference.

The experiment therefore did not expose a clear factual failure. However, it showed that agreement between AI systems is not enough to prove that an answer is correct.

### R - Reflection

I learned that two AI assistants can give similar and convincing answers, but their agreement does not automatically make the information true. Important factual claims should be checked against an independent reliable source.


## Q5 - AI Assistant vs Search vs Authoritative Reference

### A - Answer

My question was:

> Why does ice float on liquid water?

| Method | Finding |
|---|---|
| AI assistant | The AI explained that ice floats because it is less dense than liquid water. When water freezes, its molecules form a more open structure, increasing the volume and lowering the density. |
| Web search | The search results gave the same main explanation: ice is less dense than liquid water because freezing produces a more open molecular structure. |
| Authoritative reference | The U.S. Geological Survey explains that ice is less dense than liquid water and that its molecular arrangement makes the molecules more spread out. |

### E - Evidence

Authoritative reference:
U.S. Geological Survey (USGS) - Water Density
https://www.usgs.gov/water-science-school/science/water-density

### V - Verification

I compared the AI answer and web-search findings with the USGS reference. The main claims agreed. Web search was useful for finding sources, while the authoritative reference was useful for independently checking the claim.

### R - Reflection

I learned that an AI assistant can provide a quick explanation, while web search can help locate different sources. For important claims, I should check an authoritative source rather than relying only on an AI response.


## Q6 - What Is an AI Agent?

### A - Answer

| Concept | Simple explanation |
|---|---|
| LLM | A language model that processes text and generates responses based on patterns learned during training. |
| LLM application | A software application that uses an LLM to provide a useful feature such as answering questions or summarizing documents. |
| RAG system | A system that retrieves relevant information from an external source and provides it to an LLM as context. |
| Tool-using assistant | An assistant that can use external tools such as search, calculators, databases, or APIs. |
| AI agent | A system that can use a model, tools, and a workflow to perform actions toward a goal. |

Architecture:

User request
→ AI model
→ Tool call
→ Tool result
→ Model processing
→ Decision / next action
→ Final response

A simple chatbot may mainly generate a response. An agentic system can use tools, process results, make decisions, and perform multiple steps toward a goal.

Example:

A travel-planning system could search for flights, check hotel information, compare results, and create a travel plan.

### E - Evidence

I checked these definitions against the Week 1 material and a reliable technical reference.

### V - Verification

I checked especially that an agent can combine a model with tools and a workflow rather than simply generating a text response.

### R - Reflection

I learned that an LLM is only one component of a larger AI system. Agents can combine models, tools, and workflows to accomplish tasks.


## Q7 - Where Should Humans Still Make the Decision?

### A - Answer

| Situation | Possible failure | Required verification | Who/what approves? |
|---|---|---|---|
| Medical information | AI could misunderstand symptoms or provide incorrect information. | Check trusted medical information and consult a healthcare professional. | Healthcare professional |
| Financial decision | AI could use incorrect or incomplete information. | Check current financial information and relevant documents. | Human decision-maker or qualified adviser where appropriate |
| Legal information | AI could misunderstand a law or omit a requirement. | Check the relevant law or authoritative legal source. | Qualified legal professional when necessary |
| Engineering calculation | AI could make an incorrect assumption or calculation. | Recalculate and test against specifications or references. | Responsible engineer |
| Important workplace decision | AI could provide incomplete information. | Check the evidence and relevant policies. | Responsible human decision-maker |

### E - Evidence

The Week 1 material emphasizes that AI-assisted work still requires human inspection and approval, especially when incorrect output could have consequences.

### V - Verification

For each situation, I considered what could go wrong and what evidence would be needed before trusting the AI output.

### R - Reflection

I learned that AI should assist with important work rather than automatically making the final decision. The amount of verification should depend on the consequences of an incorrect result.


## Q8 - Find AI Around You

### A - Answer

| System | AI/ML involved? | Task type | Evidence/source | Conclusion |
|---|---|---|---|---|
| YouTube recommendations | Yes | Recommendation | https://support.google.com/youtube/answer/16089387 | AI/ML is used to recommend content. |
| Google Maps ETA | Yes/ML | Prediction | https://blog.google/products/maps/google-maps-101-how-ai-helps-predict-traffic-and-determine-routes/ | AI/ML is used to estimate travel time. |
| Gmail spam detection | Yes/ML | Classification | https://support.google.com/mail/answer/180707 | Machine learning is used to identify spam. |
| ChatGPT | Yes | Generation | https://openai.com/chatgpt/overview/ | It generates text responses from user prompts. |
| Phone face recognition | Yes/ML | Recognition | Not enough public evidence to conclude | I could not verify the specific AI/ML method used by my phone. |

### E - Evidence

I used public information to check whether AI or machine learning is actually involved rather than assuming that a feature is AI because it appears intelligent.

### V - Verification

I checked each example against public evidence. If public evidence is insufficient, I should record:

"Not enough public evidence to conclude."

### R - Reflection

I learned that I should not label something as AI just because it behaves intelligently. I need evidence about how the system actually works.


## Q9 - Prediction, Classification, and Generation

### A - Answer

| Example | Type | Reason |
|---|---|---|
| Predicting house prices | Prediction | Estimates a value. |
| Detecting whether an image contains a cat | Classification | Assigns the image to a category. |
| Writing an email from an instruction | Generation | Creates new text. |
| Predicting customer cancellation | Prediction | Predicts a future outcome. |
| Summarizing a research paper | Generation | Generates a new shorter text. |
| Identifying fraudulent transactions | Classification | Assigns a fraud/not-fraud category. |
| Generating an image from text | Generation | Creates new image content. |
| Predicting the next word/token | Prediction | Predicts the likely next token. |

Next-token prediction is fundamental to language models because the model can repeatedly predict the next token to generate longer text. This underlying process can support applications such as writing, summarization, coding, and question answering.

### E - Evidence

I classified each example according to its primary behavior, following the Week 1 guidance.

### V - Verification

I checked whether each example primarily predicts an outcome, assigns a category, or generates new content. I also considered that some real systems can combine multiple task types.

### R - Reflection

I learned that prediction, classification, and generation describe different AI task types. A single application can sometimes involve more than one.


## Q10 - Personal AI Verification Protocol

### A - Answer

My 7-step AI verification protocol is:

1. Define the problem — Clearly identify what needs to be solved.
2. Inspect the output — Read the AI response carefully instead of accepting it immediately.
3. Check assumptions — Identify assumptions or information that the AI may have misunderstood.
4. Check evidence and sources — Verify important factual or technical claims using reliable sources.
5. Test the result — Independently calculate, reproduce, compare, or test the result where possible.
6. Accept, reject, or revise — Decide whether the result is sufficiently supported, needs changes, or should be rejected.
7. Document and reflect — Record what was asked, what was found, how it was verified, and what remains uncertain.

### Example

I ask an AI assistant to calculate the total cost of five products. I first define which products and prices should be included. I inspect the calculation, check the assumptions and original prices, and calculate the total independently. If the result is correct, I accept it; otherwise, I revise or reject it. Finally, I record how I checked the result.

### E - Evidence

The Week 1 workflow is:

DEFINE → ASK / INVESTIGATE → INSPECT → VERIFY → CONCLUDE → DOCUMENT → REFLECT.

### V - Verification

I checked my protocol against the Q10 requirements. It includes defining the problem, inspecting assumptions, checking evidence, testing the result, deciding whether to accept/reject/revise, and documenting the process.

### R - Reflection

I learned that getting an answer from AI is only one part of the process. I should understand the problem, inspect assumptions, verify important claims, and test important results before using them.
