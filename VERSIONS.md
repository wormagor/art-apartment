# Art Apartment — Version Tracking

## Branch Structure

| Branch | Sekce | Popis |
|--------|-------|-------|
| `main` | Produkce | Finální schválená verze webu |
| `section/hero` | Hero Carousel | Titulní slideshow, nadpisy, popisky |
| `section/concept` | Concept | Unikátní koncept, popis apartmánu |
| `section/details` | Details | Specifikace, parametry apartmánu |
| `section/gallery` | Gallery | Fotogalerie a lightbox |
| `section/location` | Location | Mapa, okolí, POI |
| `section/contact` | Contact | Kontaktní formulář, booking |

## Workflow

1. **Editace sekce** → přepni na příslušnou větev (`git checkout section/hero`)
2. **Ulož verzi** → commit s popisem (`git commit -m "hero: v2 - nový podnadpis"`)
3. **Vrácení** → `git log` → `git checkout <commit-hash> -- art-apartment-v12.html`
4. **Schválení** → merge do `main` (`git checkout main && git merge section/hero`)

## Historie verzí

### main
- `cbc7e60` — Add files via upload (v12 - aktuální základ)

### section/hero
*(zatím bez změn)*

### section/concept
*(zatím bez změn)*

### section/details
*(zatím bez změn)*

### section/gallery
*(zatím bez změn)*

### section/location
*(zatím bez změn)*

### section/contact
*(zatím bez změn)*

## Konvence commit zpráv

```
<sekce>: <verze> - <popis změny>
```

Příklady:
- `hero: v2 - nový hlavní nadpis EN/CZ`
- `concept: v3 - přidány ikony vybavení`
- `location: v2 - aktualizace POI seznam`
- `contact: v4 - nový booking formulář`
