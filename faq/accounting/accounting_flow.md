# workflow

[ref issue #21](https://github.com/openfab-lab/rtfm/issues/21)

**Need:** `Login banque, Login ZOHO, Access TeamDrive/OF-Compta, *€-Rigueur-€*`

## Accounting workflow

Ce qu'on appelle par là, c'est la routine mensuelle de mettre à jour les comptes, encoder les nouveaux membres, les factures d'achats, de ventes et payer ce qu'on doit.

Pour être certain de ne pas oublier un document par ci ou une facture par là, voici une liste des tâches à suivre pour considérer que la mise à jour des comptes est faite et bien faite.

### TODOLIST

*   [ ] **SALES (ventes)**

    * [ ] [vérifier les consommations **lasersaur**](https://github.com/openfab-lab/rtfm/tree/6a59e9ed584417da711331da37e1d10734853c2c/Tools/Tools\_lasersaur\_Book.md), **LittleSebastian** (mini laser), **cnc** et **PrusaMini,** puis encoder et envoyer les factures adhoc 📑 [_create invoice_](zoho\_sales.md)
    * [ ] valider les **factures en attente** à envoyer aux membres, et aux clients si des factures récurrentes ont été créées en "draft".

    <img src="https://user-images.githubusercontent.com/12049360/54280296-6a75e400-4597-11e9-8d99-2055785496ca.png" alt="image" data-size="original">

    Il est possible de faire cette validation et d'envoyer les factures en vrac (bulk). Attention que c'est le modèle de mail automatique qui est utilisé, il n'y a pas l'étape de modification.

    <img src="https://user-images.githubusercontent.com/12049360/106891638-47083500-66eb-11eb-8f9f-fe8f2d26604b.png" alt="image" data-size="original">

    * [ ] Consulter la farde des inscriptions.\
      Au besoin, encoder les **nouveaux clients/membres.**
    * [ ] Enregistrer les **factures récurrentes** pour les cotisations à l'asbl.
* [ ] **PuuuuurCHASES (achats)**
  * [ ] **Collecter** les tickets et factures (achats par bancontact, factures, achats en ligne amazon, Aliexpress, etc... )
  * [ ] **Scanner** les docs papiers, les ajouter à la farde rouge "Achat 2019" et tout réunir sur le NAS dans `//compta/factureIN`
  * [ ] Encoder les achats déjà payés comme **Expenses (dépenses)**, avec les justificatifs en pièce jointe.
  * [ ] Encoder les achats à payer comme **Bills (factures)**, principalement des factures d'internet, douane, assurance, smartbe, etc... ainsi que notes de frais staff.
* [ ] Payer les **Bills** (factures) Aller sur le compte en ligne, et rechercher les transactions mentionnées "Open et Overdue"
*   [ ] Télécharger **les extraits**

    📑 [_import statement_](zoho\_statement.md)
* [ ] **Catégoriser** les mouvements = match entre encodage et mouvement bancaire.
* [ ] vérifier les factures envoyées et **activer les emails de rappels**

\-> wootwoot, party hard

### Remarques, astuces et récompenses

1. Une session de compta doit être complète.\
   `Exceptionnellement, si une tâche est n'est pas complétée, elle doit être traitée en priorité lors de la session suivante.`
2. La todoliste est à prendre en référence et doit pouvoir être consultée par la suite, peu importe la méthode choisie.\
   `On y retrouve les informations: qui, quand, les tâches [x] et [ ], et la méthode d'attribution du reward`
3. La reward est un montant fix de xxxx crrrr pour une todolist complète,\
   `proposition: montant à définir sur base du temps moyen d'une session x 34 x coefficient XP`

#### Astuce github:

Cette méthode manuelle est facilitée pour les utilisateurs github.\
Un template spécifique est prévu lors de la création d'une nouvelle issue dans le repo [/devis-et-facturation/issues](https://github.com/openfab-lab/devis-et-facturation/issues)

![newIssueTemplate](https://user-images.githubusercontent.com/12049360/67000753-b3b38680-f0d8-11e9-8b6d-15e30a35e881.png)

```
- [ ] **SALES**
  - [ ] vérifier le carnet lasersaur, little sebastian (minilaser), cnc 3040 et PrusaMini
  - [ ] valider les factures en attente
  - [ ] encoder les nouveaux clients/membres   
  - [ ] encoder les factures récurrentes pour inscription asbl et membership

- [ ] **PuuuuurCHASES**
  - [ ] Collecter les tickets et factures (tickets, factures, ne pas oublier achats en ligne amazon, Aliexpress, etc... )
  - [ ] Scanner les docs papiers et les ranger
  - [ ] Encoder les achats déjà payés comme **Expenses**
  - [ ] Encoder les achats à payer comme **Bills**

- [ ] Payer les **Bills**  

- [ ] Télécharger les extraits  

- [ ] Catégoriser les mouvements

- [ ] Envoyer les emails de rappel
```
