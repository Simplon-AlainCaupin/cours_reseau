**1 grande couche "application"**  

Couche 7 : 

Exemples de protocoles : HTTPS (Apache, Firefox, etc...)  
DNS (Domain Name System, eg: active directory...)  
FTP (Filezilla, sFTP, etc...)  
bit torrent...  

Exemple de requête http :

    HTTP : 
        Method URI Version CRLF  
        HEAD (Cookies : ....
              Expires : ....) CRLF  
        CRLF
        BODY => Format (eg: html, json, js, etc...)

CRLF = Carriage Return Line Feed   
(CR retour à la ligne, LF remplissage de ligne)  

En réponse on a :  

    Status-Line = HTTP-Version SP Status-Code SP Reason-Phrase CRLF  
    Headers (set-cookie : ....  
         content-length : ....) CRLF  
    BODY => (html, js ...)

eg : [status-line](https://datatracker.ietf.org/doc/html/rfc2616#section-6.1)  

