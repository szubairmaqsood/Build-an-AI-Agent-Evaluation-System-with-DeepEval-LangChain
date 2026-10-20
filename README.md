# -Build-an-AI-Agent-Evaluation-System-with-DeepEval-LangChain
https://www.youtube.com/watch?v=eL9BRo-eFYY


Build and evaluate a refund AI agent with Python, LangChain, OpenAI, and DeepEval.

It is a customer support agent that handles refund requests, then create an evaluation workflow to measure how well it performs.

The agent uses tools to look up customer purchases, check refund eligibility, calculate refund amounts, and generate simulated refund tickets. You'll connect these tools to a LangChain agent with conversation memory and structured responses.

Then we'll evaluate both the agent's answers and the actions it takes. Did it choose the right tools? Pass the correct arguments? Follow the refund policy? Complete the task without unnecessary steps?

You'll learn how to turn these questions into measurable tests using seven DeepEval metrics, inspect failures, and use the results to guide agent improvements.

By the end, you'll have an AI engineering portfolio project that demonstrates tool use, agent tracing, evaluation datasets, and data-driven iteration.

What we'll learn:

• Build a refund support agent with LangChain and OpenAI
• Define Python tools for customer lookup, date checks, refund calculations, and simulated tickets
• Add conversation memory and structured outputs with Pydantic
• Translate business rules into agent instructions and evaluation scenarios
• Create test cases with expected answers and expected tool calls
• Capture agent execution traces with DeepEval's LangChain integration
• Evaluate individual metrics before combining them into a complete workflow
• Inspect scores, pass rates, and explanations to understand failures
• Use evaluation results to improve prompts, tool use, and agent behavior

We'll explore seven evaluation metrics:

• Task completion: Did the agent accomplish the user's task?
• Step efficiency: Did it avoid unnecessary or redundant steps?
• Plan quality: Was its plan suitable for the task?
• Plan adherence: Did its execution follow the plan?
• Tool correctness: Did it call the expected tools?
• Argument correctness: Did it pass appropriate inputs to those tools?
• Answer correctness with GEval: Did its final answer reach the expected conclusion?

The project includes eight refund evaluation scenarios covering eligible refunds, purchases outside the refund window, requests for specific items, multiple-item refunds, information-only questions, missing usernames, unknown customers, and items the customer never purchased.

These cases help reveal problems that a successful demo can miss. An agent might give a convincing answer while selecting the wrong tool, calculating the wrong amount, or issuing a ticket when the user only asked a question.

We'll also discuss how to interpret evaluation failures. A low score can point to an agent mistake, an inconsistent expected answer, missing evaluation evidence, or a rubric that needs refinement. Reading the traces and explanations helps you decide what to change.

Tech stack: Python 3.12+, LangChain, LangGraph memory, OpenAI, DeepEval, Pydantic, python-dotenv, and uv.
