#🤖 Chatbot-NLP-avec-Réseau-de-Neurones-PyTorch
Ce projet implémente un chatbot conversationnel utilisant un réseau de neurones entièrement connecté développé avec PyTorch. Il traite le langage naturel via un modèle entraîné sur un jeu d’intentions défini dans intents.json et peut répondre automatiquement à des requêtes textuelles de manière interactive.

---


## 📁 Project Structure

```

├── chat.py          # Script principal pour exécuter le chatbot
├── model.py         # Définition du modèle de réseau de neurones
├── requirements.txt # Dependencies list
├── intents.json     # Base de données d'intentions et réponses
├── nltk_utils.py    # Fonctions utilitaires pour traitement du texte (tokenization, bag of words)
└── train.py         # Script d'entraînement du modèle 


````

---
##🧪 Exemple d’interaction : 

```
You: Hello
Sam: Hi there, how can I help?

You: What do you sell?
Sam: We sell coffee and tea

You: Bye
Sam: See you later, thanks for visitin


```

---
##📜 Fonctionnement : 

- Prétraitement du texte

- Les phrases sont découpées en mots (tokenization).

- Un vecteur bag-of-words est créé pour représenter chaque entrée.

- Modèle de réseau de neurones (model.py)

- 3 couches linéaires avec ReLU comme fonction d’activation.

- Classification pour prédire le tag correspondant à la phrase entrée.

- Prédiction (chat.py)

- Si la probabilité de la classe prédite est > 0.75, le bot choisit une réponse aléatoire associée à l’intention.

- Sinon, il répond par défaut : "I do not understand...".

📄 Personnalisation
Pour ajouter/modifier les réponses :

Éditez intents.json et ajoutez vos propres intentions.

Réentraînez le modèle avec votre dataset (train.py).

📝 Licence
Projet libre pour usage éducatif et expérimental. 


## 📬 Contact

📧 [yassminesaad75@gmail.com](mailto:yassminesaad75@gmail.com)
🔗 [LinkedIn – Yasmine saad](https://www.linkedin.com/in/yasmine-saad-397749278/)


