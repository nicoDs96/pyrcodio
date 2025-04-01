# pyrcodio

Una utility CLI blasfema che genera nomi combinando soggetti e attributi.

## Roadmap

- [x] **init**
- [ ] Aggiunta nomi tributo a Germano Mosconi
- [ ] Integrazione git per creare automaticamente branch con nome generato da pyrcodio
- [ ] Integrazione Docker per taggare i container con nome generato da pyrcodio

## Installazione

```
pip install pyrcodio
```

## Utilizzo

```
# Genera un singolo nome
pyrcodio

# Genera 5 nomi
pyrcodio -c 5

# Elenca le liste di parole disponibili
pyrcodio --list

# Usa liste di parole specifiche
pyrcodio -s subjects_fantasy.txt -a attributes_nature.txt

# Salva l'output su file
pyrcodio -c 10 -o names.txt

# Usa una directory dati personalizzata
pyrcodio -d /path/to/custom/data
```

## Creazione di Liste di Parole Personalizzate

Posiziona le tue liste di parole personalizzate in una directory con la seguente convenzione di denominazione:
- File dei soggetti: `subjects_*.txt`
- File degli attributi: `attributes_*.txt`

Ogni file dovrebbe contenere una parola per riga. Le righe che iniziano con # sono trattate come commenti.

## Licenza

MIT