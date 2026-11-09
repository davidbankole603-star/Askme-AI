# Askme-AI
My first AI chatbot that learns from me
brain = {
    "hi": "Hi! I'm your AI. Ask me about WAEC.",
    "who are you": "I'm an AI you built yourself.",
    "what is photosynthesis": "Plants use sunlight + water + CO2 to make food and oxygen.",
    "bye": "Bye! Go and study, future A-student."
}

print("AI is ready! Type 'hi' to start. Type 'bye' to stop.")

while True:
    question = input("You: ").lower()
    if question in brain:
        print("AI:", brain[question])
    else:
        print("AI: I don't know that yet. Teach me the answer and I'll remember it.")
        answer = input("Teach me: ")
        brain[question] = answer
        print("AI: Got it! I just learned something new.")
