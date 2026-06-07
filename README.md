# Voxirys

Assistant vocal local pour Windows : dicter du texte, lancer des commandes vocales et garder les donnees sur l'ordinateur.

Site officiel : https://voxirys.fr

## Telechargement

- Setup Windows : https://github.com/jossmair/Voxirys/raw/main/telechargements/Voxirys-Setup-0.1-beta-20260606_143947.exe
- Version portable : https://github.com/jossmair/Voxirys/raw/main/telechargements/Voxirys-Portable-0.1.zip

Voxirys est en beta. Le setup et l'archive portable peuvent etre volumineux car ils embarquent les elements necessaires au fonctionnement local.

## Ce que fait Voxirys

- Dictee vocale locale
- Commandes vocales pour piloter Windows
- Aides d'accessibilite
- Profils de dictee
- Historique et dictionnaires
- Fonctionnement CPU fiable quand CUDA n'est pas disponible

## Confidentialite

Voxirys vise un usage local : voix, texte dicte et commandes restent sur la machine. Le site rappelle clairement qu'aucune donnee n'est envoyee sur internet pour la dictee locale.

## Public vise

- Personnes ayant besoin de plus d'autonomie devant l'ordinateur
- Enseignants
- Professionnels de sante
- Utilisateurs fatigues par le clavier, la souris ou les gestes repetes

## Demarrage rapide depuis les sources

1. Installer les dependances Python du projet.
2. Lancer `Voxirys.py`.
3. Verifier le micro dans l'application.
4. Choisir un profil.
5. Utiliser `Dictee` pour ecrire ou `Commande` pour agir.

Raccourci courant : `Maj gauche` pour lancer ou arreter l'ecoute.

## Documentation utile

- Guide utilisateur : `docs/USER_GUIDE.md`
- Documentation complete : `docs/DOCUMENTATION.md`
- Premier test vocal : `docs/FIRST_RUN_DEMO.md`
- Compatibilite Windows : `docs/WINDOWS_COMPATIBILITY_REPORT.md`
- Signature Windows : `docs/AUTHENTICODE_SIGNING.md`
- Licences tierces : `docs/THIRD_PARTY_LICENSES.md`

## Qualite

Commandes de validation utilisees dans le projet :

```bash
pytest -q
python tools/run_quality_audits.py --root . --strict
python Voxirys.py --self-test
```

Avant une release publique Windows, le setup doit etre signe proprement et valide sur machine propre.

## Etat

Version actuelle : beta Windows.

Le site public et les videos de demonstration sont publies sur `voxirys.fr`.
