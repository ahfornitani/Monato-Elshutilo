# Monato-Elŝutilo

Aŭtomataj iloj (skriptoj) skribitaj per Pitono kaj PovoŜelo por elŝuti PDF-dosierojn de revuo Monato (el ties oficiala PDF-indekso ekz. <https://www.monato.be/JJJJ/pdfindex.php> )

## Pri la revuo Monato

Detalajn informojn pri la Monato oni povas legi ĉe Vikipedio: <https://eo.wikipedia.org/wiki/Monato_(gazeto)>

Kiel unu el la plej famaj kaj gravaj elementoj de la esperanta kulturo, abono certe estas rekomendinda.

Monato liberigas malnovajn eldonojn de la revuo por senpaga legado. La skriptoj do elŝutas ĉiujn tiajn dosierojn.
Dankon!

## Kiel uzi

### Per wget (plej simpla metodo)

1. Elŝutu *.txt*-dosieron `listo-de-ligiloj.txt`
2. Aliru la dosierujon per `cd` (ekz. `cd /home/ViaUzantoNomo/Downloads/MonatoPDF/` )
3. Aktivigu wget-n per `wget -i listo-de-ligiloj.txt` . Atendu kelkajn minutojn ĝis finiĝo.

Por instali wget-n oni uzu "`Scoop`"-n por *Windows* kaj "`Homebrew`"-n por *macOS*. Instruoj por instali tiujn ilojn oni facile trovas per reto-serĉilo.
Linukso jam havas ĝin (plej ofte).

### PowerShell-a skripto

Unue elŝutu la .ps1 dosieron el ĉi tiu deponejo. Memoru/notu la dosierujon, kien vi konservis ĝin. Estas tre bona ideo krei unu specifan malplenan dosierujon por la skripto kaj la elŝutotaj PDF-dosieroj. (ekz. *C:\Users\ViaUzantoNomo\Desktop\MonatoPDF* )

Se en Vindozo 10, malfermu PowerShell-on per klavumo de "WinKey + X" aŭ dekstra (cirkonstanca) alklako, kaj elektu "Windows PowerShell".
Se en malnovaj versioj, serĉu la start-menuon por "PowerShell".

Konduku PowerShell-on al la dosierujo, kie skripto konserviĝis. Ekz, se en *C:\Users\ViaUzantoNomo\Desktop\MonatoPDF* , la komando estos:
`cd 'C:\Users\ViaUzantoNomo\Desktop\MonatoPDF'`aŭ pli longe `Set-Location -Path 'C:\Users\ViaUzantoNomo\Desktop\MonatoPDF'`

Fine, la komando kiu aktivigos la skripton estas:
`.\monato-elshutilo.ps1`
Ĝi signifas: ene de la nuna dosierujo (`.\`), trovu kaj aktivigu la skripton `monato-elshutilo.ps1`

Se oni timas pri kio faras la skripto, eblas legi la kodon ĉi tie, aŭ malfermi ĝin per teksto-redaktilo (ekz. Notepad). La lineoj estas malmultaj kaj tre simplaj, do eĉ sen grandaj konoj eblas kompreni, ke ĝi estas sekura.

Eble estos necese ŝanĝi permesojn de PowerShell per [Set-ExecutionPolicy](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.security/set-executionpolicy?view=powershell-6)

![Paŝo 1](https://i.imgur.com/LFyNcof.jpg)
![Paŝo 2](https://i.imgur.com/mWpVP4b.jpg)
![Paŝo 3](https://i.imgur.com/jV0qHc8.jpg)

### Pitona skripto

Pli specife por Linukso aŭ Mac OS X (kvankam eblas ankaŭ uzi PowerShell-an version, se oni ĝin aldonis al tiuj operaciumoj).
Unue, instali kromaĵojn de Pitono per `pip install requests` .
Poste, direktu vin al dosierujo, kie estas la `.py` skripto.
Fine, aktivigu la skripton per `python ./monato-elshutilo.py`

![Python](https://i.imgur.com/HCKRIbn.jpg)

## Kiel rezigni/nuligi la elŝutadon

Se oni decidis ne elŝuti ĉiujn dosierojn, aŭ nur volas provi ĝin alimomente, la komando por nuligi estas `Ctrl+C` aŭ `Ctrl+X` (notu, ke eĉ en Mac OS oni uzu `Ctrl` anstataŭ `Cmd/⌘`
