# M300-LB3-HCL

### Inhaltsverzeichnis
* [Team  Übersicht](https://github.com/cdrc-kppr/M300-KCL#team-%C3%BCbersicht)
* [Projektbeschrieb](https://github.com/cdrc-kppr/M300-KCL#projektbeschrieb)
  * [Webserver](https://github.com/cdrc-kppr/M300-KCL#webserver-srvweb01)
  * [SQL Server](https://github.com/cdrc-kppr/M300-KCL#sql-server-srvsql01)
  * [Fileserver](https://github.com/cdrc-kppr/M300-KCL#fileserver-srvfil01)
  * [Backupserver](https://github.com/cdrc-kppr/M300-KCL#https://github.com/cdrc-kppr/M300-KCL#backupserver-srvbac01)
* [Ablage Vagrantfiles](https://github.com/cdrc-kppr/M300-KCL#https://github.com/cdrc-kppr/M300-KCL#ablage-vagrantfile)
* [Gliederung](https://github.com/cdrc-kppr/M300-KCL#gliederung)
* [K1](https://github.com/cdrc-kppr/M300-KCL#k1)
* [K2](https://github.com/cdrc-kppr/M300-KCL#k2)
* [K3](https://github.com/cdrc-kppr/M300-KCL#k3)
* [K4](https://github.com/cdrc-kppr/M300-KCL#k4)
* [K5](https://github.com/cdrc-kppr/M300-KCL#k5)



## Team Übersicht
* Luca Kiefer
* Haris Chandrakumar
* Cedric Kupper

## Projektbeschrieb 
Wir wollen 4 Virtuelle Maschinen mit der Software Vagrant in unserem Projekt umsetzen.
Folgenden Virtuelle Machienen wollte wir mit hilfe von Vagrant erstellen lassen:

#### Webserver (srvweb01)
Eine VM worauf Apache php und Wordpress installiert und kofiguriert ist. 
Das Vagrantfile sollte automatisch Wordpress, PHP und Apache installieren und dies wie folgt einrichten:
* Apache: sollte automatisch Wordpressseite erstellen
* Wordpress: sollte automatisch mit der SQL Datenbank verbunden werden die auf der VM srvsql03 liegt

#### SQL Server (srvsql01)
Eine VM worauf SQl installiert und konfiguriert ist
Das Vagrantfile sollte automatisch SQL instalieren und folgendes konfigruieren
* Datenbank namens "Wordpress" erstellen
* Wordpress user anlegen und auf Datenbank Wordpress berechtigen

#### Fileserver (srvfil01)
Eine VM auf der SAMBA installiert und Konfiguriert ist und mit den nötigen Unterordner ausgestattet.
Vagrantfile Sollte automatisch SAMBA installieren und das Konfigfile bearbeiten. Ebenfalls werden die Ordner erstellt die man Braucht.
* SAMBA: sollte automatisch installiert werden
* Ordner (HR, Buchhaltung und Leader) erstellen

#### Backupserver (srvbac01)
Eine VM die mit Debian läuft, af der ein Ordner ist der den Inhalt des Fileshares regelmässig Backuped.
Vagrantfile soll automatisc den Ordnererstellen und ein File welches für die regelmässige Ausführung des Backups sorgt.
* Odner mit Shared-Ordner Inhalt
* File welches regelmässig startet mit dem befehl zum Backup

#### Reverse Proxy
Dieser verbirgt sich normalerweise hinter der Firewall und leitet Anfragen von außen an die Backend-Server des internen Netzwerkes weiter.
Einfach gesagt ist es ein Vermittler zwischen Client und Server.
* Weiterleitung an unseren Webserver eintragen.


## Ablage Vagrantfile
Alle Vagrantfiles findet man [hier](https://github.com/cdrc-kppr/M300-KCL/tree/master/Files)


## Gliederung
Unser Markdown ist gemäss LB Anforderungen gegliedert.
Jeder Punkt ist eine LB Anforderung.

## K1

#### VirtualBox
TBZ-Cloudumgebung wird benutz, daher ist Anforderung erfüllt/installiert.

#### Vagrant
TBZ-Cloudumgebung wird benutz, daher ist Anforderung erfüllt/installiert.

#### Visualstudio-Code
TBZ-Cloudumgebung wird benutz, daher ist Anforderung erfüllt/installiert.

#### Git-Client
TBZ-Cloudumgebung wird benutz, daher ist Anforderung erfüllt/installiert.

#### SSH-Key für Client erstellt
1. SSH Key erstellen 

  * Key wird erstellt

![](images/Bild1.png)

  * Namen des Files ermitteln

![](images/Bild2.png)

  * Den Inhalt über Cat aufrufen und den Key Kopieren

![](images/Bild3.png)
  
2. SSH key auf Github hinzufügen

  * Unter SSH keys den kopierten Code einfügen.

![](images/Bild4.png)

![](images/Bild5.png)

## K2
#### GitHub oder Gitlab-Account ist erstellt
Github Accounts wurde von allen 3 Gruppenmitglieder erstellt.
Usernames
* Luca Kiefer - @luca-sk  
* Cedric Kupper - @cdrc-kppr  
* Haris Chandrakumar - @harisc1999

#### Git-Client wurde verwendet
1. SSH key-Link in die Konsole einfügen

  * In der Konsole den den git clone befehl ausführen.

![](images/Bild6.png)
  
  * Mit den richtigen logindaten anmelden.

![](images/Bild7.png)

 * (In der VM Console) Unter Source Controll das Repository Stagen und hinzufügen


#### Dokumentation ist als Mark Down vorhanden
* Siehe [hier](https://github.com/cdrc-kppr/M300-KCL)


#### Mark down-Editor ausgewählt und eingerichtet
* Siehe [hier](https://github.com/cdrc-kppr/M300-KCL)

#### Mark down ist strukturiert
* Siehe [hier](https://github.com/cdrc-kppr/M300-KCL)

#### Persönlicher Wissenstand im Bezug auf die wichtigsten Themen ist dokumentiert (Linux, Virtualisierung, Vagrant, Versionsverwaltung / Git, Mark Down, Systemsicherheit)
##### Luca Kiefer
Mit Vagrant und GitHub hatte ich persönlich noch nie zu tun. Im Modul 300 ist/war mein erster Berührungspunkt mit GitHub sowie der Virtualisierungssoftware Vagrant. 
Mit Virtualisierung sprich Azure und Hyper-V habe ich in meinem Betrieb sehr viel zu tun. Die meisten unserer Kunden besitzen einen Hyper-V Umgebung worauf viele VM laufen. Einige unserer Kunden sind mittlerweile sogar auf Azure umgestiegen. Seit rund 1 Jahr verwalte und administriere ich Azure bei Kunden.
Linux habe und konnte ich bis jetzt nur in der Schule benutzt.

##### Cedric Kupper
Leider hatte ich bis jetzt noch keinen Kontakt zu jeglicher Versionverwaltung, deshalb war Github sehr neu für mich. Vagrant ansich kannte ich zwar nicht, hatte aber wegen meiner Arbeit schon mit Virtuelen Servern bzw VMs gearbeitet. Dadurch war das Verständnis rund um Virtualisierung schon relativ gross. Linux kannte ich schon aus ÜKs und habe auch schon oft damit bei der Arbeit zu tun gehabt. Ebenfalls haben wir oft in der Schule damit gearbeitet.
Systemsicherheit ist/wird immer ein wichtigerpunkt sein, dies habe ich schon seit Lehrbeginn immer wieder gehört und gelernt. Ich kenne unterschiedlichste Wege um ein System zu Sichern.

##### Haris Chandrakumar
Ich hatte bisher leider noch nie etwas mit Vagrant und Github zutun. Da ich leider auch noch wegen dem Coronavirus am ersten Tag gefehlt habe war es umso schwerer für mich, mich dort einzufinden. Zum glück haben mir Luca und Cedric sehr geholfen mit den befehlen in Vagrant. Eine Virtualisierung zu realisieren per Skript habe ich bis jetzt noch nie gemacht. Im Betrieb habe ich mich mal eingelesen in Virtualisierung und sonst hatte ich noch einen ÜK über die Virtualisierung. Im Betrieb haben wir auch fast alles Virtuell gelöst daher konnte ich es mir vorstellen wie es funktionieren sollte.
Systemsicherheit hatte ich auch im ÜK. Das war eines der härtesten aber auch interessanteste Thema welches ich im ÜK lernen konnte.

#### Wichtige Lernschritte sind dokumentiert
##### Luca Kiefer
* 19.08.2020 
  * Vagrant kennegerlern
  * Git-Hub Account erstellelt  
  * Erste VM mit Vagrant erstellet
  * VM mit Git-Hub verbunden
* 02.09.2020
  * Vagrant selber konfiguriert und eigene VM mit hilfe von Vagrantfiles erstellt
  * Markdown bearbeitet 
  * mehrere VMs in einem File
  * Name und IP der VM mitgeben
  * Vagrant mit bootstrap file
  
##### Cedric Kupper
 * 19.08.2020
   * Vagrant kennegerlern
   * Vagrant Cloud kennengelertn
   * Git-Hub Account erstellelt  
   * Erste VM mit Vagrant erstellet
   * VM Konsole mit Git-Hub verbunden
   * SSH Key erstellt
 * 02.09.2020
   * Vagrant selber konfiguriert und eigene VM mit hilfe von Vagrantfiles erstellt
   * Markdown bearbeitet 
   * rSync kennengelernt
   * Mehrere VMs in einem File

##### Haris Chandrakumar
 * 19.08.2020
   * Vagrant kennegelernt
   * Vagrant Cloud kennengelernt
   * Git-Hub Account erstellt  
 * 02.09.2020
   * Erste VM mit Vagrant erstellt
   * VM Konsole mit Git-Hub verbunden
   * Vagrant selber konfiguriert und eigene VM mit hilfe von Vagrantfiles erstellt
 * 15.09.2020
   * VM in gemeinsamen File eingefügt


## K3
#### Bestehende vm aus Vagrant-Cloud einrichten
Mit folgedem Befehl wird einen bestehende VM aus der Vagrant Cloud inizialisiert:
vagrant init Servername/username wie zum Beispoiel ``` vagrant init ubuntu/xenial64 ```

#### Kennt die Vagrant-Befehle
Einige wichtige Vagrant befehle:
Befehl | Funktion
------------ | -------------
vagrant up | startet VM
vagrant SSH | um auf bestimmte VM zu verbinden
vagrant destroy | stopp und löscht/zerstört VM
vagrant reload | ladet die konfiguration nochmals 
vagrant halt | VM stoppen
vagrant global-status | status alles VMs
vagrant init | Erstellt VM im aktuellen Verzeichnis mit Vagrantfile falls nicht vorhanden

#### Eingerichtete Umgebung ist dokumentiert (UmgebungsVariablen, Netzwerkplan gezeichnet, Sicherheitsaspekte)

##### Namenskonvention:
SRV(Service)(Nummer)
Name | Bedeutung
------------ | -------------
srv | Server
SQL | SQL Service / Datenbank
Web | Web Service
fil | File Service
bac | Backup Service

##### Virtuelle Maschinen
Name | Funktion | Services | IP
------------ | ------------- | ------------- | ------------- 
srvweb01 | Webserver | Apache2, PHP und Wordpress | 192.168.1.10
srvsql01 | Datenbankserver | MySQL | 192.168.1.11
srvfil01 | Fileserver | SAMBA | 192.168.1.13
srvbac01 | Backupserver | - | 192.168.1.14

##### Firewall

Host | Port | IP
------------ | ------------- | ------------- 
srvweb01 | 80, 3306 | 192.168.1.10
srvsql01 | 80 | 192.168.1.11
srvfil01 | 80 | 192.168.1.13
srvbac01 | 80 | 192.168.1.14
Firewall | 80, 22 | 192.168.1.12

##### Reverse Proxy
Konfiguration Die Weiterleitungen sind in ./sites-enabled/001-reverseproxy.conf eingetragen.
Die einzige Weiterleitung die wir Konfiguriert haben ist die auf unseren Webserver (srvweb01)


##### Netwerkplan
![](images/Netzplan.PNG)

##### Sicherheitaspekte
Als unsere Sicherheit dient natürlich unsere Firewall und unser Reverse Proxy. Dank dem Reverse Proxy können die Clients nicht wissen was die tatsächliche Ip unseres Webservers ist und sind dadurch besser geschützt vor Potenziellen Angreifern. Bei unserer Firewall sind nur die Ports Offen die benötigt werden um miteinander zu kommunizieren.

#### Funktionsweise getestet inkl. Dokumentation der Testfälle andere, vorgefertigte vm auf eigenem Notebook aufgesetzt

##### SQL

Testfall  | Erwartete Aktion |Erfolgreich / nicht erfolgreich
------------ | ------------- | -------------
SQL ist installiert | SQL Konsole verfügbar -> mysql -uroot -p | erfolgreich 
SQL "Wordpress" Datenbank ist verfügbar | SHOW DATABASES ausführen; Wordpress sollte aufgelistet sein |  erfolgreich 
User Wordpress hat Berechtigung auf Wordpress Datebank | SHOW GRANTS FOR 'Wordpress'@'localhost'; Berechtigung auf Wordpress Datanbank | erfolgreich

##### Webserver

Testfall  | Erwartete Aktion |Erfolgreich / nicht erfolgreich
------------ | ------------- | -------------
Apache2 ist installiert | Apche2 Pfad vorhanden (/etc/apache2/) und service kann gestartet werden | erfolgreich
PHP ist installiert | PHP service kann gestartet werden | erfolgreich
Wordpress ist installiert | Wordpress Modul sind vorhanden | erfolgreich
Wordpressseite wurde in apache erstellt | wordpress.conf Ordner ist unter Folgendem Pfad erstellt -> /etc/apache2/sites-available/ und konfiguration ist vorhanden | erfolgreich
Wordpress ist mit Datenbank verbunden | //etc/wordpress/config-localhost.php ist konfigruriet und sql server ist hinterlegt; spich IP: 192.168.1.11 | erfolgreich
Wordpress Standard Seite ist erreichbar | Standardseite wird angezeigt | erfolgreich

Unter der folgender IP 192.168.1.1o erscheint folgende Seite (Wordpress Standardseite) - was heisst die installation war erfolgreich.
![](images/wordpress.PNG)


##### Fileserver

Testfall  | Erwartete Aktion |Erfolgreich / nicht erfolgreich
------------ | ------------- | -------------
SAMBA ist installiert | Samba konfigurationsfile / Ordner vorhanden | erfolgreich
Shared Ordner ist erstellt | Der Ordnerpfad ist erreichbar / auffindbar | erfolgreich
Die Unterordner sind erstellt | Die Unterordner sind im Sharefolder auffindbar | erfolgreich

Der Ordner ist von anderen VMs im Netzwerk erreichbar und alle Unterordner sind Eingerichtet - was heisst die installation war erfolgreich.

##### BackupServer
Testfall  | Erwartete Aktion |Erfolgreich / nicht erfolgreich
------------ | ------------- | -------------
Backupodner ist erstellt | Der Ordnerpfad ist erreichbar / auffindbar | erfolgreich
Das rSync file ist vorhanden | Das File ist unter dem entsprechenden Pfad zu finden | erfolgreich
Der rSync befehl wird regelmässig ausfgeführt | Man erstellt ein Testfile und Speichert es im Share ab, das File sollte nach 30 min im Backupordner zufinden sein. | erfolgreich

Der Backupserver sichert die Daten im Share regelmässsig (alle 30 min) - was heisst die installation war erfolgreich.

#### Projekt mit Git und Mark Down dokumentiert
Siehe [hier](https://github.com/cdrc-kppr/M300-KCL)


## K4

#### Firewall eingerichtet inkl. Rules
Für Apache Server Port 3306 aufgemacht. Und Port 80 kann von überall erreicht werden. Port 22 wird benutzt um auf unsere Firewall per SSH zugreifen zu können. Eingestellt ist auch das Default deny ist.

#### Reverse-Proxy eingerichtet
Reverse Proxy leitet Name zu unserem Webserver weiter.


#### Zugang mit SSH-Tunnel abgesichert
 * WireGuard
   Auf die VM kann nur per VPN Tunnel zugegriffen werden.
   ![](images/wireguard1.png)
   ![](images/wireguard2.png)

## K5

#### Vergleich Vorwissen - Wissenszuwachs / Reflexion

##### Luca Kiefer
Bis dahin konnte ich lernen, wie man mithilfe einer Vagrantfile mehrere Virtuelle Maschinen gleichzeitig erstellen kann.  Ausserdem weiss ich nun auch wie man die Virtuellen Maschinen, die mit Vagrant erstellt wurden, verwaltet und administriert kann.
Das kennenlernenden und später dann arbeiten mit Vagrant hat mir sehr spass gemacht. Eine solche Software kannte ich vorher nicht da ich sehr wenig mit Linux arbeite. Mit der Virtualisierung an sich werde ich in Zukunft sicherlich noch sehr viel zu tun haben, da sich die Welt nun dorthin bewegt. Viele KMUs die ich betreue sind schon auf Azure umgestiegen und beanspruchen nun alle Dienste wie Azure Aktive Directory, Azure VPN und vieles mehr von der Cloud.

Das gesamte Projekt habe ich/wir auf GitHub dokumentiert, was ich vorher nicht richtig kannte. Ich denke das Verwaltungssystem GitHub werde ich in Zukunft sicher auch öfters für mich beanspruchen, um wichtiges zu dokumentieren sowie Anleitungen und ähnliches.


##### Cedric Kupper
Ich hatte bisher nur sehr wenig Erfahrung mit Virtuellen Server umgebungen allgemein, in Vagrant gar keine. Jetzt kann ich schon sehr gut damit umgehen und einfache abläufe sind sehr schnell umgesetzt. Ich konnte durch ausprobieren, ein wenig recherche und etwas Hilfe von meinen Teamkameraden sehr viel über Vagrant dazulernen.
Auch mit Git-Hub, bzw. Versionsverwaltungstools hab ich einen besseren überblick erhalten. Nach ausprobieren und testen ging es immer besser. Mitlerweile habe ich ein gutes Grundwissen und kan relativ gut damit umgehen.

Die zusammenarbeit im Team hat sehr gut funktioniert. Die aufgaben wurden gerecht aufgeteilt und dementsprechen umgesetzt.

Das Projekt hat mich sehr gut weitergebracht. Ich denke ich werde sehr vieles davon (Vagrant und Git-Hub) in der Zukunft brauchen können. Vorallem Git-Hub, für gute, einfache und übersichtliche Dokumentationen.

##### Haris Chandrakumar
Ich hatte im Betrieb bisher nichts zutun mit Linux meine einzige Erfahrung war im ZLI und im TBZ. Durch das Modul konnte ich mein Wissen wieder auffrischen und neues dazu lernen wie zum Beispiel Vagrant und Github da ich wie am Anfang erwähnt gar keine Erfahrung mit diesen 2 Tools hatte. Doch durch Hilfe von meinen Teammitgliedern und recherche im Internet habe ich es schnell verstanden und konnte meinem Team helfen.

Ich denke ich werde in Zukunft wahrscheinlich mal wieder Github brauchen für eine Dokumentation da diese einfach ist um im Team zu bearbeiten.



