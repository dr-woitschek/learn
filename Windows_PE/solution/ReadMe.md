
**solution - Microsoft Windows PE**

---

**1. Was ist "Microsoft Windows PE"?**

Microsoft Windows PE (Preinstallation Environment) ist eine leichtgewichtige Version des Windows-Betriebssystems, die speziell für die Installation, Reparatur und Wartung von Windows-Computern entwickelt wurde. Windows PE ist kein vollständiges Betriebssystem wie Windows 10 oder Windows 11, sondern vielmehr ein minimalisiertes, bootfähiges Betriebssystem, das auf einer Windows-Kernversion basiert und auf eine einfache und effiziente Systemverwaltung abzielt.

Hier sind einige wichtige Merkmale und Verwendungszwecke von Windows PE:

1. **Installationsmedium**: Windows PE wird oft als Bootmedium verwendet, um Windows-Betriebssysteme auf neuen Computern oder Servern zu installieren. Administratoren können es auf einem bootfähigen USB-Laufwerk oder einer CD/DVD erstellen und verwenden.
2. **Reparatur- und Wartungstools**: Windows PE enthält eine Vielzahl von Diagnose- und Reparaturwerkzeugen, mit denen Probleme mit Windows-Installationen behoben werden können. Dies umfasst das Überprüfen und Reparieren des Dateisystems, das Zurücksetzen von Passwörtern, das Durchführen von Systemwiederherstellungen und vieles mehr.
3. **Datensicherung und Wiederherstellung**: Administratoren können Windows PE verwenden, um Datensicherungen durchzuführen und Daten von beschädigten oder nicht startfähigen Systemen wiederherzustellen.
4. **Image-Bereitstellung**: Windows PE wird oft in Kombination mit Tools wie dem Windows Deployment Services (WDS) oder Microsoft System Center Configuration Manager (SCCM) verwendet, um große Mengen von Windows-Images auf Computern in Unternehmen oder Organisationen bereitzustellen.
5. **Netzwerkkonnektivität**: Windows PE bietet Netzwerkkonnektivität, sodass Administratoren auf Netzwerkressourcen zugreifen, Treiber herunterladen oder Diagnosedaten an Remote-Standorte senden können.
6. **Anpassbarkeit**: Windows PE ist anpassbar, was bedeutet, dass Administratoren zusätzliche Treiber und Anwendungen hinzufügen können, um spezifische Aufgaben zu erfüllen.
7. **32-Bit und 64-Bit-Versionen**: Es gibt sowohl 32-Bit- als auch 64-Bit-Versionen von Windows PE, je nach den Anforderungen des Systems und der Aufgaben, die ausgeführt werden müssen.

Windows PE ist ein leistungsstarkes Werkzeug für IT-Administratoren und Techniker, da es ihnen ermöglicht, Systeme zu verwalten, zu reparieren und zu installieren, ohne ein vollständiges Windows-Betriebssystem auf dem Zielcomputer zu benötigen. Es ist besonders nützlich in Unternehmensumgebungen, in denen die Bereitstellung und Wartung von Windows-Computern in größerem Maßstab erfolgt.

---

**2. Was ist PXE bzw. "Preboot Execution Environment"?**

Die "Preboot Execution Environment" (PXE) ist eine Technologie und ein Protokoll, das es ermöglicht, Computer über das Netzwerk zu starten und zu booten, ohne dass ein Betriebssystem auf lokalen Massenspeichermedien installiert sein muss. PXE wird oft in Unternehmensnetzwerken, Rechenzentren und IT-Infrastrukturen verwendet, um die Remote-Verwaltung von Computern zu erleichtern und Betriebssysteminstallationen sowie Diagnose- und Wiederherstellungsprozesse durchzuführen.

Hier sind einige Schlüsselmerkmale und Verwendungszwecke von PXE:

1. **Netzwerkboot**: Mit PXE können Computer über das Netzwerk starten, indem sie eine spezielle Netzwerk-Schnittstelle (PXE-Netzwerkkarte oder PXE-fähige NIC) verwenden. Dies ermöglicht es, dass das Betriebssystem und andere Dienstprogramme direkt von einem entfernten Server geladen werden.
2. **Betriebssysteminstallation**: PXE wird häufig verwendet, um Betriebssysteme wie Windows, Linux oder andere über das Netzwerk zu installieren. Ein PXE-Server enthält Images von Betriebssystemen, die auf Client-Computer übertragen werden können.
3. **Systemdiagnose und -reparatur**: Administratoren können PXE verwenden, um auf Rettungsumgebungen und Diagnosetools zuzugreifen, um beschädigte oder nicht startfähige Systeme zu reparieren.
4. **Massenbereitstellung**: PXE ermöglicht die Massenbereitstellung von Betriebssystemen und Anwendungen auf vielen Computern gleichzeitig. Dies ist besonders nützlich in großen Unternehmensumgebungen.
5. **Zentrale Verwaltung**: PXE erleichtert die zentrale Verwaltung von Computerressourcen, da Administratoren Betriebssysteminstallationen, Updates und Reparaturen von einem einzigen Ort aus steuern können.

Der PXE-Bootvorgang funktioniert in der Regel folgendermaßen:

1. Der Client-Computer startet und initialisiert seine PXE-fähige Netzwerkkarte.
2. Die Netzwerkkarte sendet eine PXE-Anfrage (DHCP-Discover) an das Netzwerk, um nach einem PXE-Server zu suchen.
3. Ein DHCP-Server im Netzwerk antwortet auf die Anfrage und weist dem Client eine IP-Adresse zu. Der DHCP-Server kann auch Informationen über den PXE-Server bereitstellen.
4. Der PXE-Server sendet Informationen an den Client, einschließlich des Bootimages, das geladen werden soll.
5. Der Client lädt das Bootimage über TFTP (Trivial File Transfer Protocol) vom PXE-Server.
6. Nachdem das Bootimage geladen wurde, kann der Client das Betriebssystem oder Dienstprogramme von diesem Image aus starten.

PXE ist ein leistungsstarkes Werkzeug für IT-Administratoren, da es die Remote-Verwaltung und -Bereitstellung von Computern vereinfacht und zeitaufwändige manuelle Installationen über physische Medien wie DVDs oder USB-Laufwerke eliminiert. Es spielt eine wichtige Rolle in Unternehmensumgebungen, in denen effiziente und zentrale Verwaltung von Computern von entscheidender Bedeutung ist.

---

**3. Was ist ADK bzw. "Assessment and Deployment Kit"?**

Das "Assessment and Deployment Kit" (ADK) ist eine Sammlung von Tools, Dokumentation und Ressourcen, die von Microsoft entwickelt wurden, um IT-Profis bei der Bewertung, Bereitstellung und Verwaltung von Windows-Betriebssystemen und -Anwendungen in Unternehmensumgebungen zu unterstützen. Das ADK enthält verschiedene Werkzeuge, die für die Windows-Plattform entwickelt wurden und die folgenden Hauptaufgaben unterstützen:

1. **Bereitstellung von Windows**: Das ADK bietet Tools für die Bereitstellung von Windows-Betriebssystemen auf Computern in Unternehmensnetzwerken. Dazu gehören die Erstellung von Windows-Images, die Automatisierung von Installationsprozessen und die Verwaltung von Treibern.
2. **Diagnose und Fehlerbehebung**: Das ADK enthält Diagnose- und Fehlerbehebungstools, die Administratoren bei der Lösung von Problemen mit Windows-Computern und -Anwendungen unterstützen. Dies umfasst Tools zur Überprüfung und Analyse von Systemleistungsdaten.
3. **Anpassung von Windows-Images**: Mit dem ADK können IT-Profis Windows-Images anpassen, indem sie bestimmte Komponenten hinzufügen oder entfernen, Windows-Einstellungen konfigurieren und benutzerdefinierte Installationsmedien erstellen.
4. **Bereitstellung von Anwendungen**: Administratoren können das ADK nutzen, um Anwendungen und Updates in Unternehmensnetzwerken zu verteilen und zu verwalten. Dies umfasst die Erstellung von Anwendungspaketen und deren Verteilung über Gruppenrichtlinien oder Mobile Device Management (MDM)-Lösungen.
5. **Migration von Benutzerdaten**: Das ADK unterstützt auch die Migration von Benutzerdaten von alten auf neue Computer, was bei Hardware-Upgrades oder Computeraustauschen hilfreich ist.

Das ADK besteht aus verschiedenen Komponenten und Tools, darunter:

- **Windows Deployment Toolkit (WDT)**: Ein Toolkit für die automatisierte Bereitstellung von Windows, das Administratoren bei der Erstellung und Anpassung von Windows-Images unterstützt.
- **Windows Assessment Toolkit**: Ein Tool zur Bewertung der Leistung und Kompatibilität von Hardware und Anwendungen in Bezug auf Windows.
- **User State Migration Tool (USMT)**: Ein Tool zur Migration von Benutzerdaten und Einstellungen zwischen Computern.
- **Volume Activation Management Tool (VAMT)**: Ein Tool zur Verwaltung von Windows-Aktivierungs- und Lizenzierungsinformationen in Unternehmensnetzwerken.
- **Windows Performance Toolkit**: Ein Toolkit zur Leistungsanalyse und -diagnose von Windows-Systemen.

Das ADK wird regelmäßig von Microsoft aktualisiert, um die neuesten Windows-Versionen und -Funktionen zu unterstützen. IT-Profis in Unternehmen nutzen das ADK, um Windows-Bereitstellungen effizient zu verwalten, Probleme zu identifizieren und zu beheben, sowie benutzerdefinierte Windows-Images und Anwendungspakete zu erstellen und zu verteilen.

---

**4. Wie erstelle ich ein "Microsoft Windows PE"?**

Vorraussetzung: [Installiertes ADK mit PE Addon](https://docs.microsoft.com/de-de/windows-hardware/get-started/adk-install/){:target="_blank"}

starte: _"Umgebung für Bereitstellungs- und Imageerstellungstools"_ als Administrator
```
C:\Windows\system32\cmd.exe /k "C:\Program Files (x86)\Windows Kits\10\Assessment and Deployment Kit\Deployment Tools\DandISetEnv.bat" 
```

starte _"copype.cmd"_
```
Creates working directories for WinPE image customization and media creation.

copype { amd64 | x86 | arm | arm64 } <workingDirectory>
 amd64             Copies amd64 boot files and WIM to <workingDirectory>\media.
 x86               Copies x86 boot files and WIM to <workingDirectory>\media.
 arm               Copies arm boot files and WIM to <workingDirectory>\media.
 arm64             Copies arm64 boot files and WIM to <workingDirectory>\media.
                   Note: ARM/ARM64 content may not be present in this ADK.
 workingDirectory  Creates the working directory at the specified location.

Example: copype amd64 C:\WinPE_amd64
```

starte _"makewinpemedia.cmd"_
```
Creates bootable WinPE USB flash drive or ISO file.

MakeWinPEMedia {/ufd | /iso} [/f] <workingDirectory> <destination>
 /ufd              Specifies a USB Flash Drive as the media type.
                   NOTE: THE USB FLASH DRIVE WILL BE FORMATTED.
 /iso              Specifies an ISO file (for CD or DVD) as the media type.
 /f                Suppresses prompting to confirm formatting the UFD
                   or overwriting existing ISO file.
 workingDirectory  Specifies the working directory created using copype.cmd
                   The contents of the <workingDirectory>\media folder
                   will be copied to the UFD or ISO.
 destination       Specifies the UFD volume or .ISO path and file name.

 Examples:
   MakeWinPEMedia /UFD C:\WinPE_amd64 G:
   MakeWinPEMedia /UFD /F C:\WinPE_amd64 H:
   MakeWinPEMedia /ISO C:\WinPE_x86 C:\WinPE_x86\WinPE_x86.iso
```
