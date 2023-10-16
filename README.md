# Alphavision-ML
Node-red SIA naar MQTT

Flow SIA koppeling Alphatronics ML

De flow is gemaakt op de basis van het 
SIA protocol. omdat het mij niet lukte
ok de standaard integratie werkend 
te krijgen heb ik deze flow gebouwd
de standaard integratie doet de 1e 
bericht afhandeling en zorgt dat de
centrale ook een antwoord krijf=gt waardoor 
deze uit storing blijft.

Door het binnen komend bericht te filteren
en te splitsen ben ik tot een bericht gekomen 
welke ik via MQTT door stuur naar Home-Assisant

Welke berichten zijn verwerkt
Voor de Zones:
/CL = Inschakelen Zone
/OP	= Uitschakelen Zone
/BA = Inbraak alarm
/FA = Brand Alarm

Algemeen:
/RP = Centrale - Controle bericht
/AT = Centrale - storing voeding AC
/YT = Centrale - Storing Accu
/BC = Centrale - Melding Hersteld door gebruiker
