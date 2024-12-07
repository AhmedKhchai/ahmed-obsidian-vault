- Add slide numbers.
- Answer correctly about ISO 31000.
- Explicitly say that we're presenting a risk matrix.
	- Explicit that they're global risks & IT risks.
- Add legends to the PCA, re-evaluate priorities.
- Propose a simple Carto that mentionnes Security and data collection form "les metier".
- Re-evaluate the RSE, maybe mention it during the "Gouvernance SI".
- Mention multi-lingual Veille Techno.
- Add titles to sub-processes, re-evaluate linear processes.
- Add a annex menu.

## Proposition Cartographie
	CRM, mobilité et accès centralisé (SSO), ainsi que des contraintes métiers incluant la sécurité, la conformité RGPD, l'intégration des systèmes existants, et la gestion des stocks.
According to the needs we collected from les metiers we suggest an infrastructure cartographie that is secured (DMZ, VPN, Security and Redundency Measures).  Take an example of the ERP that will be shared by Spain and France (RH, Finance, Referentiel Data) and plan integration with existing software.

En fonction des besoins recueillis auprès des métiers, nous proposons une cartographie de l'infrastructure sécurisée (DMZ, VPN, mesures de sécurité et de redondance).  Prenons l'exemple de l'ERP qui sera partagé entre l'Espagne et la France (RH, Finance, Données référentielles) et prévoyons une intégration avec les logiciels existants.

```
[Internet]
    |
    |----------------------[Pare-feu Externe]----------------------
    |                         /                 \                  |
[DMZ]                 [Pare-feu Interne]   [Réseau Interne]
    |                      /       |       \                     |
[Serveur Web]   [VLAN RH] [VLAN Finance] [VLAN Production]
    |                   
    |                              [VPN Site-à-Site]
    |                                      |
[Serveur DNS]-------------------[VPN Gateway]
    |                                      |
[Serveur Mail]                          [France Office]
    |
[IDPS]
    |
[Antivirus/Anti-malware Solutions]

```

### Infrastructure Proposal for ERP Integration

#### 1. **Current Environment Analysis**

- **France and Spain Sites**: Existing IT infrastructure in France (main) and Madrid (secondary).
- **Key Systems**: ERP for Finance and HR in France, customized systems for production and e-commerce.
- **Security Posture**: Current systems with limited security measures, no centralized security policy, fragmented backup and recovery processes.

#### 2. **Proposed Secure Infrastructure**

1. **Network Segmentation and DMZ Implementation**
    
    - **DMZ Setup**: Create a DMZ to host public-facing services like web servers, email servers, and DNS servers. This isolates these services from the internal network, reducing the risk of external attacks.
    - **Internal Network Segmentation**: Use VLANs to segment the network into functional areas (HR, Finance, Production, etc.), enhancing security and performance.
2. **VPN for Secure Communication**
    
    - **Site-to-Site VPN**: Implement a secure VPN connection between the French and Spanish sites to ensure encrypted data transmission.
    - **Remote Access VPN**: Provide secure remote access for employees working from different locations or from home.
3. **Security Measures**
    
    - **Firewalls**: Deploy firewalls at each site to control incoming and outgoing traffic, with strict rules for DMZ, VPN, and internal network communication.
    - **Intrusion Detection and Prevention Systems (IDPS)**: Implement IDPS to monitor and block suspicious activities.
    - **Antivirus and Anti-malware Solutions**: Install comprehensive endpoint protection on all servers and workstations.
4. **Redundancy and High Availability**
    
    - **Server Redundancy**: Implement redundant servers for critical services to ensure high availability.
    - **Data Backup and Recovery**: Establish a robust backup strategy with regular backups and off-site storage. Implement a disaster recovery plan with defined RTO and RPO.
5. **Integration with Existing Systems**
    
    - **ERP Integration**: Integrate the ERP system with existing systems in both France and Spain, ensuring seamless data flow and process alignment.
    - **Data Synchronization**: Use data synchronization tools to keep reference data, HR, and Finance information consistent across both sites.
6. **Monitoring and Management**
    
    - **Centralized Monitoring**: Deploy a centralized monitoring system to oversee network performance, security incidents, and system health.
    - **Performance Dashboards**: Create dashboards to monitor key performance indicators (KPIs) such as system uptime, network latency, and security alerts.
7. **User Training and Support**
    
    - **ERP Training**: Conduct comprehensive training sessions for users on the new ERP system and integrated processes.
    - **Ongoing Support**: Provide continuous support through a dedicated helpdesk and regular system updates.

- ### Proposition d'Infrastructure Sécurisée en 7 Points Clés

1. Créer une DMZ pour héberger les services accessibles au public, isolant ainsi le réseau interne des attaques externes.
2. Utiliser des VLANs pour segmenter le réseau interne en zones fonctionnelles (RH, Finance, Production) pour améliorer la sécurité et les performances.
3. Mettre en place un VPN site-à-site sécurisé entre la France et l'Espagne pour garantir la transmission chiffrée des données.
4. Fournir un accès VPN sécurisé pour les employés travaillant à distance ou depuis leur domicile.
5. Déployer des systèmes de détection et de prévention des intrusions (IDPS) pour surveiller et bloquer les activités suspectes.
6. Mettre en place des serveurs redondants pour les services critiques afin d'assurer une haute disponibilité.
7. Organiser des sessions de formation complètes pour les utilisateurs sur le nouveau système ERP et fournir un support continu via une assistance dédiée.



Politique de gestion des équipements en fin de vie : Mise en place de donation d’équipement IT

Certification verte : Fournisseure certifié ISO 14 001 et ISO 26000

Conditions de travail et bien-être des salariés : Offrir des services de conseil psychologique et encourager des activités sociales et des groupes de soutien en entreprise.
