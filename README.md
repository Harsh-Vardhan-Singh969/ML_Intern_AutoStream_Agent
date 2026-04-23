# ML_Intern_AutoStream_Agent
AI chatbot agent for AutoStream using LangChain with RAG, intent detection, and lead capture simulation.

### How to run

1. Clone the repository 
2. Install required packages
pip install -r requirements.txt
3. Open file chatbot.ipynb in google colab 
4. Run all cells 
5. start_chat()

---

### Chatbot architecture

The chatbot consists of three components: Intent Detection, RAG with defined knowledge base, and lead capturing.

Intent detection is performed using rules to define whether a query is greeting, informative, or high-intent.

RAG retrieves information from the knowledge base to make sure that answers are correct.

State management is performed using memory buffer, containing up to 5-6 turns of conversation.

In case a high intention is detected from user, the chatbot captures lead information including name, email, and platform.

---

### Integration with WhatsApp

It is possible to integrate this chatbot with WhatsApp using WhatsApp Cloud API.

Messages from users will be received through webhook, processed using the chatbot, and responded back.

Lead information can be saved in databases such as Firebase or PostgresSQL.
