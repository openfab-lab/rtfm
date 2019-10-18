# workflow

[ref issue \#21](https://github.com/openfab-lab/rtfm/issues/21)

**Need:** `Login banque, Login ZOHO, Access TeamDrive/OF-Compta, Access OpenfabNAS, *€-Rigueur-€*`

## Accounting workflow

Ce qu'on appelle par là, c'est la routine mensuelle de mettre à jour les comptes, encoder les nouveaux, les achats, les ventes et payer ce qu'on doit.

Pour être certain de ne pas oublier un document par ci ou une facture par là, voici une liste des tâches à suivre pour concidérer que la mise à jours des comptes est faite et bien faite.

### TODOLIST

* [ ] **SALES**

  * [ ] [vérifier le **carnet laser**](https://github.com/openfab-lab/rtfm/tree/6a59e9ed584417da711331da37e1d10734853c2c/Tools/Tools_lasersaur_Book.md), encoder et envoyer les factures adhoc 📑 [_create invoice_](zoho_sales.md)
  * [ ] valider les **factures en attente** à envoyer aux membres, aux clients si des factures récurrentes on été créée en "draft"

  ![image](https://user-images.githubusercontent.com/12049360/54280296-6a75e400-4597-11e9-8d99-2055785496ca.png)

  * [ ] Au besoin, encoder les **nouveaux clients/membres**.   
  * [ ] Enregistrer les **factures récurrentes** pour inscription asbl et membership

* [ ] **PuuuuurCHASES**
  * [ ] **Collecter** les tickets et factures \(achats par bancontact, factures, achats en ligne amazon, Aliexpress, etc... \)
  * [ ] **Scanner** les docs papiers, les ajouter à la farde rouge "Achat 2019" et tout réunir sur le NAS dans `//compta/factureIN`
  * [ ] Encoder les achats déjà payé comme **Expenses**, avec en pièce jointe les justificatifs.
  * [ ] Encoder les achats à payer comme **Bills**, principalement des factures d'internet, douane, assurance, smartbe, etc... ainsi que note de frais staff.
* [ ] Payer les **Bills** Aller sur le compte en ligne, et enregistrer les virements "Open et Overdue"
* [ ] Télécharger **les extraits**   

  📑 [_import statement_](zoho_statement.md)

* [ ] **Catégoriser** les mouvements = match entre encodage et mouvement bancaire.
* [ ] vérifier les factures envoyée et **activer les email de rappels**

-&gt; wootwoot, party hard

### Remarques, astuces et récompenses

~~cheat-sheet du code de la TODOLIST, copypasta de ceci dans l'issue de la tâche,~~

#### Attention:

Cette méthode manuelle est dépréciée.   
Un template spécifique est prévu lors de la création d'une nouvelle issue dans le repo [/devis-et-facturation/issues](https://github.com/openfab-lab/devis-et-facturation/issues)

![newIssueTemplate](https://user-images.githubusercontent.com/12049360/67000753-b3b38680-f0d8-11e9-8b6d-15e30a35e881.png)

```text
- [ ] **SALES**
  - [ ] vérifier le carnet laser
  - [ ] valider les factures en attente
  - [ ] encoder les nouveaux clients/membres   
  - [ ] enregistrer les factures récurrentes pour inscription asbl et membership

- [ ] **PuuuuurCHASES**
  - [ ] Collecter les tickets et factures (tickets, factures, ne pas oublier achats en ligne amazon, Aliexpress, etc... )
  - [ ] Scanner les docs papiers et les ranger
  - [ ] Encoder les achats déjà payé comme **Expenses**
  - [ ] Encoder les achats à payer comme **Bills**

- [ ] Payer les **Bills**  

- [ ] Télécharger les extraits  

- [ ] catégoriser les mouvements

- [ ] activer les email de rappels
```

