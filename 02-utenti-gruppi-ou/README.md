# Modulo 02 - Utenti, Gruppi e Organizational Units

## Obiettivo
Creare e organizzare utenti e gruppi in Active Directory 
tramite Organizational Units, applicando best practice 
di sicurezza nella gestione delle identità.

## Procedura

### 1. Creazione Organizational Units
Create due OU per separare logicamente utenti e gruppi:
- `LAB_UTENTI` — contiene gli account utente
- `LAB_GRUPPI` — contiene i gruppi di sicurezza

![Creazione OU LAB_UTENTI](screenshots/ou-utenti.png)
![Creazione OU LAB_GRUPPI](screenshots/ou-gruppi.png)

### 2. Creazione utenti
Creati tre utenti nella OU `LAB_UTENTI`:

| Username | Nome | Tipo |
|----------|------|------|
| M.Rossi | Mario Rossi | Utente standard |
| G.Bianchi | Giulia Bianchi | Utente standard |
| Admin.Test | Admin Test | Account privilegiato |

![Creazione utente](screenshots/creazione-utente.png)
![Utenti nella OU](screenshots/unità-utenti.png)

Best practice applicata: **"Cambiamento password 
all'accesso successivo"** su tutti gli account — 
garantisce che solo l'utente conosca la propria password.

![Impostazione password](screenshots/imposta-password.png)


### 3. Creazione gruppi
Creati due gruppi di sicurezza nella OU `LAB_GRUPPI`:

| Gruppo | Ambito | Tipo | Scopo |
|--------|--------|------|-------|
| GRP_Utenti_Standard | Globale | Sicurezza | Utenti standard del dominio |
| GRP_Amministratori | Globale | Sicurezza | Account con privilegi elevati |

Scelto il tipo **Sicurezza** invece di Distribuzione 
per poter assegnare permessi alle risorse del dominio.

![Creazione gruppo](screenshots/creazione-gruppo.png)
![Gruppi nella OU](screenshots/unità-gruppi.png)

### 4. Assegnazione utenti ai gruppi

| Gruppo | Membri |
|--------|--------|
| GRP_Utenti_Standard | Mario Rossi, Giulia Bianchi |
| GRP_Amministratori | Admin Test |

Separazione tra utenti standard e account privilegiato — 
applicazione del principio di **Least Privilege**: ogni 
utente ha solo i permessi necessari al proprio ruolo.

![Membri GRP_Utenti_Standard](screenshots/gruppo-utentistandard.png)
![Membri GRP_Amministratori](screenshots/gruppo-utentiadmin.png)

## Risultato
Struttura AD organizzata con OU, utenti e gruppi. 
Gli utenti standard sono separati dall'account 
privilegiato sia a livello di OU che di gruppo.

## Snapshot
`03-Utenti-Gruppi-OU` — stato del sistema 
al termine del modulo.

## Collegamento con Security+
- **Least Privilege** (SY0-701 – 2.3): separazione 
  utenti standard da account privilegiati
- **AAA** (SY0-701 – 1.2): gestione centralizzata 
  delle identità tramite AD
- **Identity and Access Management** (SY0-701 – 4.6): 
  gruppi di sicurezza per controllo degli accessi
