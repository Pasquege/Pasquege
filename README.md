- 👋 Hi, I’m @Pasquege
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Pasquege/Pasquege is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import tkinter as tk
import random

# Lista di frasi d'amore
frasi_amore = [
    "Ti amo!",
    "Sei la mia felicità!",
    "Il mio amore per te è infinito!",
    "Sei il mio sogno diventato realtà!",
    "Sei la luce della mia vita!",
    "Ogni istante con te è prezioso!",
    "Il tuo sorriso mi fa innamorare ogni giorno!",
    "Sei il mio tutto!"
]

# Funzione per generare una frase d'amore casuale
def genera_frase_amore():
    frase = random.choice(frasi_amore)
    label_frase.configure(text=frase)

# Creazione della finestra
finestra = tk.Tk()
finestra.title("Frase d'Amore")
finestra.geometry("800x800")

# Etichetta per visualizzare la frase d'amore
label_frase = tk.Label(finestra, text="", font=("Arial", 24))
label_frase.pack(pady=100)

# Pulsante per generare una nuova frase d'amore
pulsante_genera = tk.Button(finestra, text="Genera Frase", command=genera_frase_amore, font=("Arial", 16))
pulsante_genera.pack()

# Avvia il loop principale della finestra
finestra.mainloop()
