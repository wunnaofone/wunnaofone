def math_bot():
    print("Hello! I’m MathBot. Ask me a math question.")
    while True:
        question = input("You: ")
        if question.lower() in ["exit", "quit"]:
            print("MathBot: Goodbye!")
            break
        
        try:
            answer = eval(question)
            print(f"MathBot: The answer is {answer}")
        except Exception as e:
            print("MathBot: Sorry, I couldn't understand that. Please try again.")

if __name__ == "__main__":
    math_bot()
