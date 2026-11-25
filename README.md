# Présentation interactive — technologies du diabète

> **État constaté : maquette HTML incomplète, non exécutable comme présentation fonctionnelle.** Les deux fichiers HTML inspectés s'arrêtent au milieu d'une déclaration CSS, sans corps de document ni logique de présentation.

## Architecture constatée

```mermaid
flowchart LR
 CDN[Chart.js JSZip FileSaver references] --> Draft[Incomplete HTML and CSS]
 Draft --> Missing[Presentation body and logic absent]
```

[index.html](index.html) et [seconde maquette](presentation%20medtronic.html) référencent des bibliothèques CDN et définissent des styles d'interface, mais ne contiennent ni moteur de boucle fermée, ni graphique initialisé, ni export ZIP opérationnel, ni contrôle d'accès établi. Des styles de modal ou de navigation ne prouvent pas leur implémentation. Cette maquette indépendante n'est ni une application médicale ni une communication officielle de Medtronic.

Qualification proposée : retrouver ou reconstruire la présentation à partir de contenus autorisés et sourcés, compléter le document HTML, vérifier les attributions et les liens. Ne pas utiliser pour programmer un dispositif médical. Aucun test, appel CDN ou déploiement réalisé.

## English overview

This independent diabetes-technology presentation repository contains two incomplete HTML/CSS drafts that end mid-declaration, with external library references but no implemented presentation body or interactive logic. It does not implement a closed-loop medical device or validated clinical material and is not affiliated with Medtronic. No runtime validation was performed.

[Notice de droits](LICENSE.md) : droits et marques tiers préservés.


**Catégorie : santé, vulgarisation & présentation technique** · Studio Niko Design

Ce dépôt contient une maquette web indépendante incomplète sur les technologies liées au diabète et aux systèmes en boucle fermée. Le fichier `index.html` se présente comme « NIKO AI | Global Engineering Pack » et charge notamment Chart.js, JSZip et FileSaver.js.

## Consulter la présentation

Examiner le code de `index.html` ; la présentation doit être complétée avant utilisation. Pour tester le projet avec un serveur local :

```bash
python3 -m http.server 8000
```

Accéder ensuite à http://localhost:8000/.

## Structure

- `index.html` — maquette principale incomplète.
- `presentation medtronic.html` — autre fichier de présentation HTML.
- `README.md` — description et précautions.

## Dépendances

Le code charge des bibliothèques JavaScript et des styles via CDN. Une connexion peut être nécessaire et la disponibilité des services tiers n'est pas garantie.

## Précautions importantes

**Présentation indépendante, non officielle et non affiliée à Medtronic.** Les noms de marques et de produits appartiennent à leurs propriétaires. Ce dépôt n'est ni un dispositif médical ni une source de conseil thérapeutique, et ne doit pas servir à programmer une pompe ou à ajuster un traitement. Vérifier les spécifications et recommandations auprès de sources officielles et de professionnels de santé.

**Statut :** contenu de démonstration ; les références techniques, chiffres et compatibilités doivent être revus avant tout usage professionnel ou clinique.

[Retour au catalogue Studio Niko Design](https://github.com/Nikoju1977).
