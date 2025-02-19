
**solution - Batch**

---

```

@echo off
cls
echo.
echo 1. ausgefuehrter Commandline Befehl ............................................. "%CmdCmdLine%"
echo 2. von wo wird das Batch-Script ausgefuehrt, Laufwerk und den kompletter Pfad ... "%~dp0"
echo 3. von wo wird das Batch-Script ausgefuehrt, nur das Laufwerk ................... "%~d0"
echo 4. von wo wird das Batch-Script ausgefuehrt, nur den Ordner ..................... "%~p0"
echo 5. Dateiname der ausgefuehrten Datei ohne Dateiwerweiterung ..................... "%~n0"
echo 6. Dateierweiterung der ausgefuehrten Datei ..................................... "%~x0"
echo 7. Ausgefuehrte Datei mit Ordner ................................................ "%~f0"
echo.
pause

```

![Screenshot - cmd](https://github.com/dr-woitschek/learn/blob/main/Batch/solution/cmd.jpg)

---
