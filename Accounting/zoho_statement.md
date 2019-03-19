[ref issue #3](https://github.com/openfab-lab/rtfm/issues/3)

# "Statement": c'est quoi?
C'est les extraits de compte. Les lignes de mouvements IN/OUT, les sous qu'on reçoit et qu'on donne.  
On a besoin de ça pour valider les opérations que l'on encode dans Zoho et c'est mieux d'aller chercher ça sur son compte en ligne plutôt que de tout écrire à la main.

J'ai créé un tableur qui va trier et ordonner comme il faut les datas venant du compte. Au final, ça doit reprendre ceci:

Date | Withdrawals | Deposits | Payee | Description | Reference Number
-- | -- | -- | -- | -- | --
`=importBpost!$B2` | `=Abs(if(importBpost!$D2>0;0;importBpost!$D2))` | `=if(importBpost!$D2<0;0;importBpost!$D2)` | `=importBpost!$H2` | `=importBpost!$I2` | `=importBpost!$A2`
2019-01-17 | 538,17 | 0 | EXP GmbH | order .334001 at EXP Tech | 28
2019-01-16 | 0 | 45,00 | Ciklic | Velom2 abon. guilde | 27
2019-01-14 | 0 | 60,00 | LAURENT | OF-B085 | 26
2019-01-11 | 40,51 | 0 | PROXY BRUXELLES | 20190111 09:14:00 | 25

## How to import statement from bankAccount
1. **Download** last statement from Account page
2. **Import** this .csv into the spreadsheet  **xchange-BPO2ZOHO** on drive/OF-Comptabilité
![image](https://user-images.githubusercontent.com/12049360/52051422-d7876a00-2553-11e9-9a2a-2b02af18c207.png)

3. **Sort data A>X**
![image](https://user-images.githubusercontent.com/12049360/52051744-b2472b80-2554-11e9-96ff-618ba62b30f8.png)

4. Very well, now, take care to **delete already added values!**  
On évite ainsi cette erreur : ![image](https://user-images.githubusercontent.com/12049360/52076556-34544600-258f-11e9-856e-e98135eebbcf.png)

5. Then, we can find everything we need to export to zoho in the **next sheet**
![image](https://user-images.githubusercontent.com/12049360/52052732-9c873580-2557-11e9-93c4-05bc1fe0aafe.png)

6. **export to csv**
![image](https://user-images.githubusercontent.com/12049360/52052761-b759aa00-2557-11e9-9030-eeb0488d03ce.png)


## .CSV checking
Oui, parce que la vie c'est dur, et que les ordinnateurs ne font jamais vraiment exactement ce qu'on veut. _ça serait trop facile, gniiiii_  

### Par exemple.
Certains bidules vont pourrir l'import dans ZOHO.


**Les caractères spéciaux**  
un peu comme ici:
![image](https://user-images.githubusercontent.com/12049360/54288771-4ec70980-45a8-11e9-9f1e-94a39714c654.png)  

un carré est ajouté lors de l'export et remplace l'espace marquant les "milliers".   

**Les €**  
il faut vérifier que les données de valeurs ne sont pas considérées comme du texte et que le

**Les -**  
ben oui, parce qu'il y a une colonne débit et une colonne crédit alors toutes les valeurs sont positives. _shuuuuuut, don't ask, c'est un truc de comptable_

## Back in Zoho books
- **Import Statement**
![image](https://user-images.githubusercontent.com/12049360/52052819-e5d78500-2557-11e9-8356-4605501a3eef.png)

- **Charger le fichier .csv** et laisser tout comme ça.
![image](https://user-images.githubusercontent.com/12049360/52052885-1b7c6e00-2558-11e9-9a93-cf348b72306e.png)

- Everything should **match automatically** since We use the expected names.
![image](https://user-images.githubusercontent.com/12049360/52052938-449cfe80-2558-11e9-8252-5bce77da7485.png)

![image](https://user-images.githubusercontent.com/12049360/54630877-1f6a3e00-4a7b-11e9-9a05-749488bd0a74.png)

---
---
Next thing will be to categorize these new transactions.
![image](https://user-images.githubusercontent.com/12049360/52053001-6b5b3500-2558-11e9-8551-3f895bdf2a25.png)
