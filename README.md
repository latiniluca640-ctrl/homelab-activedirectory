# Home Lab - Active Directory

Home Lab personale progettato per simulare una piccola 
infrastruttura aziendale.
Il laboratorio viene utilizzato per sperimentare 
configurazioni di rete, Active Directory, hardening, 
monitoraggio, automazione e sicurezza informatica, 
documentando ogni attività come se fosse un ambiente reale.

## Obiettivo
Realizzare un laboratorio domestico che simuli una piccola 
infrastruttura aziendale per esercitarmi su tecnologie di 
amministrazione di sistema, networking e cybersecurity.
Ogni modulo documenta la configurazione, le motivazioni 
delle scelte e le verifiche effettuate, con l'obiettivo 
di consolidare competenze pratiche e creare un portfolio 
tecnico consultabile.

## Ambiente
- Hypervisor: VirtualBox
- OS: Windows Server 2022 Standard Evaluation
- Ruolo principale: Domain Controller (lab.local)

## Moduli
| # | Modulo | Stato |
|---|--------|-------|
| 01 | Installazione Windows Server e configurazione DC | ✅ Completato |
| 02 | Utenti, Gruppi e Organizational Units | ✅ Completato |
| 03 | Group Policy | ✅ Completato |
| 04 | Kali Linux — Setup, configurazione e test di sicurezza progressivi | ⏳ Pianificato |
| 05 | NPS / RADIUS | ⏳ Pianificato |
| 06 | PKI e Active Directory Certificate Services | ⏳ Pianificato |
| 07 | Segmentazione di rete e pfSense | ⏳ Pianificato |
| 08 | VM Client Windows | ⏳ Pianificato |
| 09 | Mail server interno — SPF, DKIM, DMARC | ⏳ Pianificato |
| 10 | Sysmon, Audit Logging e DLP | ⏳ Pianificato |
| 11 | Wazuh SIEM — ELK Stack, Zabbix, SNMP, MIB e ntopng | ⏳ Pianificato |
| 12 | Metasploitable — Test infrastruttura difensiva | ⏳ Pianificato |
| 13 | Ansible — Automazione configurazioni e patch | ⏳ Pianificato |

## Note
- Questo repository è in continua evoluzione —
  nuovi moduli vengono aggiunti man mano che
  vengono affrontati durante lo studio.
- `GPO_Defender` e `GPO_Firewall` da aggiungere al modulo 03
- Wazuh girerà su VM Debian dedicata — macchina di gestione del lab

## Certificazioni collegate
- CompTIA Security+ SY0-701 (in corso)
