

Prompt Engineering Lab

The Prompt Engineering Lab serves as an Education and Experimentation Hub provided by The Generative Intelligence Lab @ FAU. Prompt Engineering is a rapidly evolving discipline at the intersection of Artificial Intelligence (AI) and Natural Language Processing (NLP). This lab is designed to help students, researchers, and developers experiment with the art of creating and refining prompts, offering easy-to-follow resources and opportunities to contribute, collaborate, and share their work.

Prompt Engineering has emerged as a critical component in unlocking the full potential of language models such as Phi, LLaMA, and Qwen. As AI systems continue to revolutionize problem-solving, mastering how to guide and optimize these models through effective prompting techniques is essential for cutting-edge research, practical applications, and future innovation.

This lab provides a hands-on learning environment where participants can actively apply their knowledge through Python code, Jupyter notebooks, and practical exercises designed to foster both experimentation and discovery.

Configure Your Lab Environment

Before starting, configure your lab environment:

General Audience Configuration

FAU Students Configuration

Troubleshooting Guide

Prompt Engineering Techniques

Explore various prompt engineering techniques:

Zero-Shot Prompting

Few-Shot Prompting

Prompt Template

Chain-of-Thought Prompting

Meta Prompting

Self-Consistency Prompting

More techniques coming soon!

Want to contribute? Check out the Contributing Guide.

Experimenting with Prompt Engineering

Once your lab environment is set up (see configuration guide), you can start experimenting with built-in Prompt Engineering techniques or create your own experiments by modifying the provided code.

(1) Adjust the Incoming Prompt (Simulating User/System Requests)

MESSAGE = "What is 2 * log(10)?"

(2) Modify the Prompt Engineering Technique (Simulating Workflow Templates)

TEMPLATE_BEFORE = "Act like you are a math teacher\nYour student is asking:"
TEMPLATE_AFTER = "Give only the answer; refrain from any more information"
PROMPT = TEMPLATE_BEFORE + '\n' + MESSAGE + '\n' + TEMPLATE_AFTER

(3) Configure the Model Request (Simulating Workflow Orchestration)

Documentation on available parameters: Ollama API Docs

payload = create_payload(target="ollama",
                         model="llama3.2:latest",
                         prompt=PROMPT,
                         temperature=1.0,
                         num_ctx=100,
                         num_predict=100)

References

Meta - Prompting Guide

OpenAI Prompting Engineering Guide

Ollama API Documentation

Open WebUI API Endpoints

