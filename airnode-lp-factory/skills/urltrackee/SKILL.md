---
name: urltrackee
description: Genere des URLs de test avec parametres de tracking realistes pour Google Ads, Meta, LinkedIn et Bing. Utiliser quand on teste le tracking UTM d'une LP.
---

# Generateur d'URLs trackees de test

Quand l'utilisateur donne une URL, generer **4 URLs de test** avec des parametres de tracking realistes.

Si l'URL contient deja un `?`, utiliser `&`. Ne PAS ajouter `_fbc`, `_fbp` ni les parametres de consentement (ce sont des cookies).

## Google Ads
```
utm_source=google&utm_medium=cpc&utm_campaign=test-google-2026&utm_content=rsa-v1&utm_term=mot+cle+test&campaign_id=21547893210&adgroup_id=164892357401&ad_id=698745231058&gclid=EAIaIQobChMIz7qN8pu4jAMVkZloCR0mXAFcEAAYASAAEgKVUvD_BwE&gbraid=CLjVxcCEz7qN8pu4jAMVkZloCR0mXAFc&wbraid=EgYwAoD3xNKiz7qN8pu4jAMVkZloCR0
```

## Meta (Facebook)
```
utm_source=facebook&utm_medium=paid-social&utm_campaign=test-meta-2026&utm_content=carousel-v1&fbclid=IwAR3xK7mN2vL8pQ9dR5sT1uW0yA4bC6eF8gH3jI2kL5mN7oP0qR4sT6uV&meta_platform=facebook&meta_placement=feed
```

## LinkedIn Ads
```
utm_source=linkedin&utm_medium=paid-social&utm_campaign=test-linkedin-2026&utm_content=single-image-v1&li_fat_id=a9b8c7d6-e5f4-3a2b-1c0d-9e8f7a6b5c4d
```

## Microsoft Ads (Bing)
```
utm_source=bing&utm_medium=cpc&utm_campaign=test-bing-2026&utm_content=rsa-v1&utm_term=mot+cle+test&msclkid=abc123def456ghi789jkl012mno345pqr678stu901
```

Afficher les 4 URLs completes pretes a copier-coller.
