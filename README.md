# Neovim Befehle

# 💾 Speichern

- `:w` – speichern
- `ZZ` – speichern + schließen  
- `:sav file` – speichern unter

# 📌 Motions

- `h` – nach links  
- `l` – nach rechts  
- `j` – nach unten  
- `k` – nach oben  

- `w` – zum nächsten Wort  
- `b` – zum vorherigen Wort  
- `e` – zum Wortende springen  

- `$` – zum Ende der Zeile  
- `0` – zum Anfang der Zeile  
- `^` – zum ersten Nicht-Leerzeichen  

- `f s` – zum nächsten 's'  
- `t s` – vor das nächste 's'  

- `}` – nächster Absatz  
- `{` – vorheriger Absatz  

- `Ctrl + f` – eine Seite vor  
- `Ctrl + b` – eine Seite zurück  
- `Ctrl + d` – halbe Seite runter  
- `Ctrl + u` – halbe Seite hoch  

- `Ctrl + e` – scroll down  
- `Ctrl + y` – scroll up  

- `zt` – Cursor oben  
- `zb` – Cursor unten  

- `gg` – Anfang Datei  
- `G` – Ende Datei  

- `10gg` / `:10` – gehe zu Zeile 10  

- `Ctrl + o` – zurück (jumplist)  
- `Ctrl + i` – vorwärts  

- `H` – oben im Screen  
- `M` – Mitte im Screen  
- `L` – unten im Screen

# ⚙️ Operatoren
- `I` – Anfang Zeile + Insert  
- `A` – Ende Zeile + Insert  

- `o` – neue Zeile darunter  
- `O` – neue Zeile darüber  

- `u` – undo  
- `Ctrl + r` – redo  

- `r` – Zeichen ersetzen  

# ❌ Delete
- `d` – delete operator  
- `de` – bis Wortende löschen  
- `dw` – bis nächstes Wort löschen  
- `dd` – ganze Zeile löschen  
- `D` – bis Zeilenende löschen  
- `x` / `X` – Zeichen löschen  

- `:%d` – ganze Datei löschen  

- `d$` – bis Zeilenende  
- `d0` – bis Zeilenanfang  

- `3dw` – 3 Wörter löschen  
- `10dj` – 10 Zeilen löschen  

- `C` – bis Zeilenende löschen + Insert  

- `di(` – Inhalt in Klammern löschen  

# 📋 Copy & Paste

y    - kopieren
p    - einfügen

yiw  - Wort kopieren
yy   - Zeile kopieren
dd   - Zeile ausschneiden

p / P  - darunter / darüber einfügen

v    - Visual Mode
V    - Line Mode
Ctrl + v  - Block Mode

R    - Replace Mode

# 🔍 Suchen

- `/search` – vorwärts  
- `?search` – rückwärts  

- `n` / `N` – next / prev  
- `*` / `#` – Wort unter Cursor  

- `/search\c` – case insensitive

# 🔁 Ersetzen

- `:s/a/b/` – einmal ersetzen  
- `:s/a/b/g` – ganze Zeile  
- `:%s/a/b/g` – ganze Datei  
- `:%s/~/$HOME/g` – ersetzen  

# 📦 Register & Zwischenablage

- `y` – kopieren  
- `p` – einfügen  

- `yiw` – Wort kopieren  
- `yy` – Zeile kopieren  
- `dd` – Zeile ausschneiden  

- `p` / `P` – darunter / darüber einfügen  

- `v` – Visual Mode  
- `V` – Line Mode  
- `Ctrl + v` – Block Mode  

- `R` – Replace Mode

# 📑 Tabs

- `:tabnew file` – neuer Tab  
- `gt` / `gT` – wechseln  
- `:tabclose` – schließen

# 🪟 Splits / Fenster

- `Ctrl + w h/j/k/l` – wechseln  
- `Ctrl + w v` – vertikal  
- `Ctrl + w s` – horizontal  
- `Ctrl + w c` – schließen  

- `Ctrl + w +` / `Ctrl + w -` – Größe ändern  
- `Ctrl + w =` – ausgleichen  

# 📂 Buffer

- `:e file`     – öffnen
- `:buffers`    – anzeigen
- `:b name`     – wechseln
- `:bd`         – schließen
- `:bn / :bp`   – next / prev
- `:bw` 

# 🧠 Jump List

- `ma` – Mark setzen  
- `Ctrl + o` – zurück  
- `Ctrl + i` – vor

# 📍 Marks

- `:marks` – anzeigen  
- `ma` – setzen  
- `` `a `` – springen  
- `:delmarks a` – löschen

# 📦 Folds

- `zM` – alle schließen  
- `zR` – alle öffnen  
- `za` – toggle  
- `zc` – schließen  
- `zo` – öffnen

# ⚡ Funktionen

- `:.w !bash` – Zeile ausführen  
- `:exec '!'.getline('.')` – extern ausführen  

- `:e` – reload file

# 🔧 Häufige Aufgaben

- `ggVG` – alles markieren  
- `:%s/^\s\+//` – führende Leerzeichen entfernen  
- `:sort` – sortieren  

- `:set number` – Zeilennummern anzeigen  
- `:set relativenumber` – relative Zeilennummern  

- `:checktime` – neu laden

# 🔁 Makros

- `qa` – aufnehmen  
- `q` – stoppen  

- `@a` – abspielen

# 🧪 Sonstiges

- `~` – case toggle  
- `>>` – einrücken  
- `<<` – ausrücken  

- `gi` – zurück zum Insert  
- `.` – wiederholen  
- `Ctrl + a` / `Ctrl + x` – Zahl erhöhen / verringern  
- `:set list` / `:set nolist` – Anzeige von Whitespaces ein/aus

# 🔢 Zahlen generieren

- `:put =range(1,10)`  

- `:put =map(range(1,150), 'printf(''%04d'', v:val)')`  

- `:for i in range(1,10) | put ='192.168.0.'.i | endfor`  



