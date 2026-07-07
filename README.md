<div align="center">
  <img src="assets/voxirys-launcher.png" alt="Voxirys" width="88">

  # Voxirys

  **Reconnaissance vocale locale pour Windows.**  
  Dictee vocale, commandes Windows et souris a la voix, sans cloud obligatoire.

  [Site officiel](https://voxirys.fr/) |
  [Telecharger](https://voxirys.fr/download.html) |
  [Reconnaissance vocale](https://voxirys.fr/reconnaissance-vocale.html)
</div>

---

## Telecharger la beta

Voxirys est en beta pour Windows 10 et Windows 11.

| Version | Lien |
| --- | --- |
| Setup Windows recommande | [Telecharger le setup](https://github.com/jossmair/Voxirys/raw/main/telechargements/Voxirys-Setup-0.1-beta-20260606_143947.exe) |
| Version portable | [Telecharger l'archive portable](https://github.com/jossmair/Voxirys/raw/main/telechargements/Voxirys-Portable-0.1.zip) |
| Empreintes | [CHECKSUMS.txt](CHECKSUMS.txt) |

Les fichiers sont volumineux parce que Voxirys embarque des elements necessaires au fonctionnement local.

## Ce que fait Voxirys

- Dicter du texte dans les applications Windows.
- Lancer des commandes vocales simples.
- Aider au clic et aux interactions avec la souris a la voix.
- Reduire les gestes repetes au clavier et a la souris.
- Garder la voix et les textes dictes sur l'ordinateur autant que possible.

## Pour qui

Voxirys vise surtout les usages ou la voix rend l'ordinateur plus simple ou plus confortable :

- accessibilite et fatigue clavier-souris ;
- enseignement, preparation de notes et corrections ;
- sante, administratif et contextes sensibles ;
- utilisateurs qui veulent tester une reconnaissance vocale locale sur Windows.

## Confidentialite

Voxirys privilegie un fonctionnement local. L'objectif est que la voix, les commandes et les textes dictes restent sur la machine, sans dependance cloud obligatoire.

Voir : [docs/CONFIDENTIALITE.md](docs/CONFIDENTIALITE.md)

## Demarrage rapide

1. Telechargez le setup Windows.
2. Installez Voxirys.
3. Ouvrez l'application.
4. Verifiez le micro.
5. Lancez la dictee ou le mode commande.

Guide : [docs/INSTALLATION.md](docs/INSTALLATION.md)

## Etat du projet

Voxirys est encore en beta. Les retours utiles concernent surtout l'installation, le micro, la reconnaissance vocale, l'ergonomie, l'accessibilite et les cas metier.

Pour aider le projet :

- testez la beta ;
- ajoutez une etoile au depot si le projet vous interesse ;
- partagez [voxirys.fr](https://voxirys.fr/) avec les personnes qui cherchent une dictee vocale locale pour Windows ;
- ouvrez une issue avec votre contexte d'usage.

## Developpement

Commandes de validation utilisees pendant le developpement :

```bash
pytest -q
python tools/run_quality_audits.py --root . --strict
python Voxirys.py --self-test
```

Avant une diffusion plus large, le setup Windows devra etre signe proprement et valide sur machine propre.
