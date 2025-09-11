# Étape 1 : utiliser une image Python légère
FROM python:3.11-slim

# Définir le dossier de travail dans le conteneur
WORKDIR /app

# Copier le fichier requirements.txt s'il existe
COPY requirements.txt .

# Installer les dépendances
RUN pip install --no-cache-dir -r requirements.txt

# Copier tout le code de l’application
COPY . .

# Exposer le port Flask (par défaut : 5000)
EXPOSE 5000

# Commande pour lancer ton app Flask
CMD ["python", "app.py"]
