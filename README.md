# A02U - Activitat 2 - DHCP a Win 2020 Server

mp07-uf01-02-dhcp-win2020

## Objectiu

Instal·lació i configuració del **```servei de DHCP```** en un servidor **Windows 2020 Server**.

## Eines

Per tal de dur a terme la pràctica la instal·lació s'implementarà sobre una màquina **Windows 2020 Server**. També caldrà que connecteu el vostre servidor amb dues màquines virtuals client de dos companys.


## Ajuda

Al repositori [xuleta-markdown](https://github.com/joanpardogine/xuleta-markdown), trobareu informació sobre les comandes a fer servir a **```markdown```**.

## Procediment

**1.** Cal crear un **repositori remot** (en el vostre compte de **```github```**) anomenat:

**```<CognomAlumne>-mp07-uf01-02-dhcp-win2020```**

on **```<CognomAlumne>```** serà **només** el vostre **cognom** **sense el nom**. Per exemple, en el meu cas seria **```pardo-mp07-uf01-02-dhcp-win2020```**.

**2.** Cal que el **repositori remot** sigui **```privat```**.

**3.** Cal que convideu a l'usuari **```joanpardogine```** al **repositori remot**.

En el fitxer **```README.md```** haureu de crear una taula (feta amb **```markdown```**) amb la informació de quins son els companys amb el que connectareu el vostre servidor.

## Passos per realitzar l'activitat

Aquests passos cal que quedin reflectits al fitxer **```README.md```** del vostre **repositori remot**. Per a cadascun dels passos cal que afegiu una explicació de com heu fet cada pas. I si es possible una captura de pantalla.  

**1.** Cal que modifiqueu el nom del vostre servidor. El nom d'aquest cal que sigui **```<CognomAlumne>smx2```**, on **```<CognomAlumne>```** serà **només** el vostre **cognom** **sense el nom**. Per exemple, en el meu cas seria **```pardosmx2```**.

> Cal que afegiu una explicació de com heu fet aquest pas, i si es possible una captura de pantalla al fitxer **```README.md```** del vostre **repositori remot**.

**2.** Cal verificar que el vostre servidor disposa de **dues interfícies de xarxa**:

   * la primera interfície de xarxa que donarà sortida a Internet (**```NAT```**)

   * la segona interfície de xarxa caldrà que m'expliqueu con cal configurar-la, per poder-la connectar amb les dues màquines virtuals amb un sistema operatiu client dels vostres companys. Aquesta segona interfície de xarxa tindrà una IP fixa de la subxarxa
        **```172.128.<mesDelVostreAniversari>.0/24```**

> Cal que afegiu una explicació de com heu fet aquest pas, i si es possible una captura de pantalla al fitxer **```README.md```** del vostre **repositori remot**.

**3.** El vostre **```servidor DHCP```** assignarà de manera **fixa** (*caldrà fer una reserva*) l'adreça IP **```172.128.<mesDelVostreAniversari>.55/24```** a una de les interfícies de xarxa de la màquina client d'un dels vostres companys. Cal que esbrineu quina MacAddress té la interfície de xarxa del client.

> Cal que afegiu una explicació de com heu fet aquest pas, i si es possible una captura de pantalla al fitxer **```README.md```** del vostre **repositori remot**.

**4.** El **rang d'adreces IP** que assignarà el nostre servidor **DHCP**, anirà des de l'adreça IP:

 * **```172.128.<mesDelVostreAniversari>.50```**, fins a la
 
 * **```172.128.<mesDelVostreAniversari>.150```**.

> Cal que afegiu una explicació de com heu fet aquest pas, i si es possible una captura de pantalla al fitxer **```README.md```** del vostre **repositori remot**.

**5.** Les **adreces dels servidors de DNS** que assignarà el vostre **servidor DHCP**, cal que siguin les **DNS de google**.

Com a Sistema Operatiu client podreu fer servir qualsevol que tingui la possibilitat de configurar la interfície de xarxa perquè rebi la configuració de xarxa de forma automàtica.

> Cal que afegiu una explicació de com heu fet aquest pas, i si es possible una captura de pantalla al fitxer **```README.md```** del vostre **repositori remot**.

## Contingut

Segons la vostra pròpia informació i formació

## Lliurament

Com ja s'ha comentat, cal que afegiu una explicació de com heu fet cada pas, i si es possible una captura de pantalla al fitxer **```README.md```** del vostre **repositori remot** i a part el professor passarà un a un per veure-ho de manera presencial.

Al final de l'explicació, caldrà que el fitxer **```README.md```** del vostre **repositori remot**, contingui en **format text** els següents continguts:

**1.** el **nom del vostre servidor** (***hostname***),

**2.** el resultat de la comanda **```ipconfig /all```** (**en format text**), de:

   **2.1.** el vostre **servidor**,

   **2.2.** de les dues màquines client dels vostres companys.

**3.** Quines són i com heu aconseguit les **dns de google**.