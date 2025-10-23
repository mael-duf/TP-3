# TP 3
### Génération d’une requête ARP
```ping -c 1 10.2.0.255```

<img width="560" height="166" alt="image" src="https://github.com/user-attachments/assets/ec817615-2919-412c-8522-45852d83d823" />

```sudo tcpdump -n -e arp```

<img width="874" height="135" alt="image" src="https://github.com/user-attachments/assets/61a43176-b478-4c22-8e4a-5701cfb55efc" />

## 

### Consultation de la table ARP
```apr -a```

<img width="578" height="483" alt="image" src="https://github.com/user-attachments/assets/163c579e-5d04-4bc9-aebd-ad759781b572" />

### Question : 
#### 1_ L'entrée qui est ajoutée correspond à l’IP de PC2 et son adresse MAC
#### 2_ En général, sa dure 1 a 3 minutes

## 

### Analyse avec Wireshark
### Quelle est la différence entre ARP Request et ARP Reply ? 
####L’ARP Request est une demande en broadcast pour trouver l’adresse MAC d’une IP, tandis que l’ARP Reply est la réponse de la machine concernée envoyée en unicast avec son adresse MAC.

### Quelle machine envoie la réponse ?
#### PC 2

## 
### Simulation d’un empoisonnement ARP
### Analyse le risque : comment l’attaquant devient-il “homme du milieu” ?
#### le trafic peut passer par l’ordinateur de l’attaquant au lieu d’aller à la bonne destination. C’est comme si quelqu’un au milieu du réseau détournait tes messages pour les lire ou les modifier.
