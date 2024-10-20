import random

# Réponses du chatbot
responses = {
    "salut": "Salut! Comment puis-je t'aider?",
    "comment ça va?": "Ça va bien, merci! Et toi?",
    "quel est ton nom?": "Je suis un simple chatbot sans nom.",
    "au revoir": "Au revoir! Passe une bonne journée!"
}

def chatbot_response(user_input):
    return responses.get(user_input.lower(), "Je ne comprends pas...")

# Boucle de conversation
print("Parle avec moi! (Tape 'au revoir' pour quitter)")
while True:
    user_input = input("Tu: ")
    if user_input.lower() == "au revoir":
        print("Chatbot: Au revoir! Passe une bonne journée!")
        break
    print("Chatbot:", chatbot_response(user_input))

