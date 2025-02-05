# Ontologi LLM Classifier

Ce projet utilise une ontologie des domaines du droit et un modèle de langage pour classifier des textes juridiques.

## Prérequis

- Python 3.9+
- [Pydantic](https://pydantic-docs.helpmanual.io/)
- [OpenAI SDK](https://github.com/openai/openai-python)
- Un fichier `domaines-demo.json` contenant l'ontologie (il s'agit d'une classification de démonstration)

## Utilisation

Le script charge l'ontologie depuis `domaines-demo.json`, définit des modèles de données avec Pydantic et envoie un prompt au modèle OpenAI (gpt-4o) pour effectuer une opération de matching et retourner 3 labels avec leurs probabilités.

Exécutez le script avec :

```bash
python classify_droit.py
