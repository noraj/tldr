# vim

> Vim (Vi IMproved), een command-line tekst bewerker, geeft toegang tot verschillende manieren van tekst manipulatie.
> Drukken op `<i>` begint invoegmodus. `<Esc>` begint normale modus, wat toegang geeft tot de Vim commando's.
> Bekijk ook: `vimdiff`, `vimtutor` en `nvim`.
> Meer informatie: <https://www.vim.org>.

- Open een bestand:

`vim {{pad/naar/bestand}}`

- Open een bestand bij een bepaald regelnummer:

`vim +{{regelnummer}} {{pad/naar/bestand}}`

- Bekijk de handleiding van Vim:

`<:>help<Enter>`

- Opslaan en afsluiten:

`{{<Esc><Z><Z>|<Esc><:>x<Enter>|<Esc><:>wq<Enter>}}`

- Terug naar normale modues en maak de laatste verandering ongedaan:

`<Esc><u>`

- Zoek een patroon in het bestand (druk op `<n>`/`<N>` om naar de volgende/vorige overeenkomst te gaan):

`</>{{zoek_patroon}}<Enter>`

- Voer een reguliere expressie substitutie uit in het hele bestand:

`<:>%s/{{reguliere_expressie}}/{{vervanging}}/g<Enter>`

- Geef de regelnummers weer:

`<:>set nu<Enter>`
