**Minecraft Java Plugin**

---

**Hello World**

- Über den Befehl `org.bukkit.Bukkit.getConsoleSender().sendMessage("Text");` können wir Meldungen auf der Konsole ausgeben.<br/>Wir fügen den Befehl in den Bereich `public void onEnable()` ein.<br/>Dieser wird beim laden des Plugins abgearbeitet.
  Hier ein Beispiel:
  ```
  public void onEnable() {
      // Plugin startup logic
      org.bukkit.Bukkit.getConsoleSender().sendMessage("   ____  ____  ____  ____                           ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage("  /\\   \\/\\   \\/\\   \\/\\   \\                  ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage(" /  \\___\\ \\___\\ \\___\\ \\___\\                 ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage(" \\  / __/_/   / /   / /   /                        ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage("  \\/_/\\   \\__/\\/___/\\/___/                     ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage("    /  \\___\\    /  \\___\\     Plugin Spielplatz  ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage("    \\  / __/_mc_\\  /   /      von Dr. Woitschek   ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage("     \\/_/\\   \\/\\ \\/___/                        ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage("       /  \\__/  \\___\\         Version 1.0        ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage("       \\  / _\\  /   /                             ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage("        \\/_/\\ \\/___/                             ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage("          /  \\___\\                                ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage("          \\  /   /                                 ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage("           \\/___/                                  ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage("                                                    ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage("         Hallo Welt                                 ");
      org.bukkit.Bukkit.getConsoleSender().sendMessage("                                                    ");
  }
  ```
  ![Screenshot](https://github.com/dr-woitschek/minecraft/blob/main/JavaEdition/Plugins/Level1-Hello-World/Bilder/IntelliJ_IDEA_01.jpg)

- Über den `Play`-Button können wir das Testen
  ![Screenshot](https://github.com/dr-woitschek/minecraft/blob/main/JavaEdition/Plugins/Level1-Hello-World/Bilder/IntelliJ_IDEA_02.jpg)

- Die Befehle `getLogger().info("Text");` bzw. `getLogger().warning("Text");` zeigen Info- bzw. Warn-Meldungen an.
  Hier ein Beispiel:
  ![Screenshot](https://github.com/dr-woitschek/minecraft/blob/main/JavaEdition/Plugins/Level1-Hello-World/Bilder/IntelliJ_IDEA_03.jpg)

---

_Weitere Informationen_
- [https://www.jetbrains.com/de-de/](https://www.jetbrains.com/de-de/)
- [https://papermc.io/](https://papermc.io/)
