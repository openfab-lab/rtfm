[ref issue #21](https://github.com/openfab-lab/rtfm/issues/21)

**Need:** `Login banque, Login ZOHO, Access TeamDrive/OF-Compta, Access OpenfabNAS, *€-Rigueur-€*`

# Accounting workflow
Pour être certain de ne pas oublier un document par ci ou une facture par là, voici une liste des tâches à suivre pour concidérer que la mise à jours des comptes est faite et bien faite.  

## TODOLIST
- [ ] **SALES**
  - [ ] [vérifier le **carnet laser**](/Tools/Tools_lasersaur_Book.md), encoder et envoyer les factures adhoc
  - [ ] valider les **factures en attente** à envoyer aux membres, aux clients si des factures récurrentes on été créée en "draft"
    - [ ] Au besoin, encoder les **nouveaux clients/membres**.   
  - [ ] Enregistrer les **factures récurrentes** pour inscription asbl et membership

- [ ] **PuuuuurCHASES**
  - [ ] **Collecter** les tickets et factures (achats par bancontact, factures, achats en ligne amazon, Aliexpress, etc... )
  - [ ] **Scanner** les docs papiers, les ajouter à la farde rouge "Achat 2019" et tout réunir sur le NAS dans `//compta/factureIN`
  - [ ] Encoder les achats déjà payé comme **Expenses**, avec en pièce jointe les justificatifs.
  - [ ] Encoder les achats à payer comme **Bills**, principalement des factures d'internet, douane, assurance, smartbe, etc... ainsi que note de frais staff.

- [ ] Payer les **Bills**  
 Aller sur le compte en ligne, et enregistrer les virements "Open et Overdue"

- [ ] Télécharger **les extraits**  
_-> [import statement](/Accounting/zoho_statement.md)_

- [ ] **Catégoriser** les mouvements = match entre encodage et mouvement bancaire.

- [ ] vérifier les factures envoyée et **activer les email de rappels**

-> wootwoot, party hard

---

## Remarques, astuce et récompenses

cheat-sheet du code de la TODOLIST, copypasta de ceci dans l'issue de la tâche, nom= "Accounting + `date`"

```
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
