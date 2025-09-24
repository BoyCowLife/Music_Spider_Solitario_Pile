# 🎵 Scale Master - Quiz Musicale PWA

Un gioco educativo Progressive Web App per imparare le scale maggiori musicali, ispirato alla meccanica del solitario Spider.

## 📱 Caratteristiche

- **PWA completa** - Installabile su iOS/Android come app nativa
- **Design verticale** ottimizzato per mobile
- **Offline-first** - Funziona senza connessione
- **3 livelli di difficoltà**:
  - Facile: 3 scale
  - Medio: 4 scale
  - Difficile: 5 scale
- **Drag & Drop** ottimizzato per touch
- **13 scale maggiori** con alterazioni (diesis e bemolle)

## 🎮 Come si gioca

1. Il gioco estrae casualmente 3-5 scale maggiori (in base alla difficoltà)
2. Ogni scala mostra i 7 gradi (I-VII) come slot vuoti
3. Clicca sulla carta coperta per rivelare una nota
4. Trascina la nota nel grado corretto della scala appropriata
5. Completa tutti i gradi di tutte le scale per vincere!

## 🚀 Installazione su GitHub Pages

1. Fai fork di questo repository
2. Vai in Settings → Pages
3. Seleziona "Deploy from a branch"
4. Scegli branch `main` e cartella `/ (root)`
5. Salva e attendi il deploy (circa 2-3 minuti)
6. La tua app sarà disponibile su: `https://[tuo-username].github.io/scale-master/`

## 📲 Installazione su iOS

1. Apri Safari su iPhone/iPad
2. Naviga all'URL della tua app
3. Tocca il pulsante condividi (quadrato con freccia)
4. Scorri e seleziona "Aggiungi alla schermata Home"
5. Dai un nome all'app e tocca "Aggiungi"

## 🛠️ Struttura File

```
scale-master/
│
├── index.html          # App principale
├── manifest.json       # PWA manifest
├── sw.js              # Service Worker
├── icon.svg           # Icona sorgente
├── icon-192.png       # Icona PWA 192x192
├── icon-512.png       # Icona PWA 512x512
└── README.md          # Documentazione
```

## 🎨 Generazione Icone PNG

L'icona SVG inclusa può essere convertita in PNG usando:

### Opzione 1: Convertitore Online
- Vai su [CloudConvert](https://cloudconvert.com/svg-to-png)
- Carica `icon.svg`
- Imposta dimensioni: 192x192 e 512x512
- Scarica e rinomina: `icon-192.png`, `icon-512.png`

### Opzione 2: PowerShell + Inkscape
```powershell
# Installa Inkscape prima
inkscape icon.svg --export-width=192 --export-height=192 --export-filename=icon-192.png
inkscape icon.svg --export-width=512 --export-height=512 --export-filename=icon-512.png
```

## 🎼 Scale Disponibili

- **Con diesis**: C, G, D, A, E, B, F♯
- **Con bemolle**: F, B♭, E♭, A♭, D♭, G♭

## 🔧 Personalizzazione

Puoi modificare facilmente:

- **Colori**: Cambia il gradiente in CSS
- **Difficoltà**: Modifica `getNumberOfScales()` in JavaScript
- **Scale**: Aggiungi/modifica in `scalePatterns`
- **Animazioni**: Personalizza le transizioni CSS

## 📄 Licenza

MIT License - Usa liberamente per progetti personali o educativi!

## 🎸 Per Chitarristi Jazz

Perfetto per chi sta imparando l'improvvisazione! Le scale maggiori sono la base per:
- Modi (Dorico, Frigio, Lidio, etc.)
- Progressioni II-V-I
- Sostituzione di accordi
- Walking bass

## 🐛 Troubleshooting

**L'app non si installa su iOS?**
- Assicurati di usare Safari (non Chrome)
- Verifica che il manifest.json sia servito correttamente

**Il drag & drop non funziona?**
- Verifica che il browser supporti touch events
- Prova a ricaricare la pagina

**Non funziona offline?**
- Attendi che il Service Worker si registri (primo caricamento)
- Ricarica la pagina una volta

---

Creato con ❤️ per musicisti e programmatori