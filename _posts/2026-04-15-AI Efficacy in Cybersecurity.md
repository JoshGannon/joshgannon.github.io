# How I've leveraged AI Agents in Cybersecurity for actual productivity gains

Within this field of work, we are managing hardware and software.  These are deterministic and have volumes of documentation, which is an ideal combination for leveraging LLMs.

Using company-approved tooling, AI agents are very easy to create and fine-tune. What is not easy - and where career experience is essential - is knowing when the AI is prone to hallucinate and where to apply guardrails to ensure success.

## Easy AI Agent creation
With HatzAI for example, simply click to create a new agent, choose the AI Tool Selectors (Firecrawl, Perplexity, etc), define the Instructions Field (agent's directive like AV or firewall vendor expert, KB or internal documentation), and test for viability/usefulness.

## Examples where fine-tuning these AI Agents requires experience

LLM Verbosity and noise:

In testing and where a vendor has much documentation, LLMs tended to be overly cautious and far to verbose for Cybersecurity topics. Within the Instructions Field, a directive can be added such as 'be concise'.  We humans are the subject matter expert and are the final line for decision-making - the LLMs can be leveraged to scour volumes of documentation and condense relevant information.

Firmware version control:

In testing where needing a product firmware version where a bug is resolved, AI agents tend to check the most recent release notes and recommend the bleeding edge version. It takes experience to know that firmware version control is in play and to add a directive to the AI agent to specify that when recommending a firmware version, specify the fixed firmware within the major and minor release and prefer a maintenance release when possible.

## Summary
Since these tools are generally leveraged by whole teams, it has been very beneficial in my experience to fine-tune these AI Agents to allow us to scale productivity while maintaining system security, accuracy, and stability. AI agents aren’t replacing expertise; they’re amplifying it.
