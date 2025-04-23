# Portfolio
Afin de témoigner de ma motivation et de permettre au recruteur de voir un aperçu de qui je suis j'ai décider de faire un portfolio assez design 
Mon nom de domain : https://ericanebajagan.com

BUT : Faire une site Portfolio totalement sécurisé (pas de Wget, Curl, BrutForce, ect) 

POUR LA SECURISATION :
1. reCAPTCHA de Google (recommandé)
Le plus utilisé et gratuit.

Intégration :
On va sur  : https://www.google.com/recaptcha

Tu choisis v2 (case à cocher) ou v3 (invisible)

Tu récupères ta clé de site et ta clé secrète

Tu ajoutes le script dans ton HTML :

<script src="https://www.google.com/recaptcha/api.js" async defer></script>
<form action="verif.php" method="POST">
  <div class="g-recaptcha" data-sitekey="TA_CLÉ_SITE"></div>
  <input type="submit" value="Accéder au site">
</form>

Et dans verif.php, tu vérifies la réponse avec la clé secrète.

- Authentification sécurisée (bcrypt, reCAPTCHA, 2FA possible)
- Protection contre les injections SQL / XSS / CSRF
- Vérification des fichiers uploadés (type, taille, extensions)
- HTTPS avec certificat SSL
- Gestion des sessions et cookies sécurisés
- Rate limiting / protection brute-force sur l’accès admin
- Journalisation des connexions et erreurs suspectes
- Scan de vulnérabilités automatisé (ex. : OWASP ZAP) Avec nikito, Wappalyzer
- Google Analytics afin d'obtenir les statistiques
- Faire rapport de sécurité avec les tests réalisés ect..


