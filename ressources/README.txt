Il faut modifier la ligne d'option pour indiquer le chemin du script d�pos� juste avant :
DAEMON_ARGS="/opt/teleinfo/teleinfo.py -e IP_DE_JEEDOM -c CLE_API_DE_JEEDOM"
Le rendre �x�cutable : chmod +x /etc/initd.d/teleinfo
L'ajouter au boot : update.rc-d /etc/initd.d/teleinfo defaults
Et le faire d�marrer : service teleinfo start