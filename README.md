# 📦 Discord Bot - Modular avec Cogs

Ce projet est un bot Discord développé avec **discord.py**, organisé en **Cogs** pour une structure claire et évolutive.

## 🔧 Installation

1. **Cloner le repo**

```bash
git clone <url-du-repo>
cd <nom-du-projet>
```

2. **Installer les dépendances**

```bash
pip install -r requirements.txt
```

3. **Configurer le bot**

Modifier le fichier `config.json` :

```json
{
  "token": "TON_TOKEN",
  "prefix": "!",
  "developper": "123456789012345678",
  "version": "1.0.0",
  ...
}
```

> 💡 Assure-toi que le token est bien celui de ton bot, et que les ID sont valides.

## 🚀 Lancer le bot

```bash
python main.py
```

## 📁 Structure du projet

```
.
├── main.py               # Point d'entrée du bot
├── cogs/                 # Commandes organisées par module
│   ├── vcpv.py           # Gestion vocaux persos
│   ├── lock.py           # Commandes lock/unlock
│   ├── privacy.py        # pv / unpv
│   ├── clear.py          # Suppression de messages
│   ├── help.py           # Système de help interactif
│   └── commands_config.py # Slash commands: addcommand / removecommand
├── config.json           # Configuration du bot
├── utils/
│   └── io_utils.py       # Fonctions load/save pour les fichiers JSON
```

## 🛠 Fonctions principales

- `vcpv` → Création / suppression / gestion de salons vocaux persos
- `lock`, `unlock` → Contrôle de l'accès aux salons texte
- `pv`, `unpv` → Rendre un salon privé ou public
- `clear` → Nettoyage de messages avec limite configurée
- `help` → Système d'aide avec embed + navigation
- `addcommand`, `removecommand` → Gestion dynamique du help

## 🙏 Remerciements

- [discord.py](https://github.com/Rapptz/discord.py)
- Ton imagination ✨

---

Prêt à faire tourner ton bot sur ton serveur !


