# Pokedex Lite

App móvil hecha con **React Native + TypeScript** (Expo y Expo Router) que consume la [PokeAPI](https://pokeapi.co/).

## Pantallas (rutas)

| Ruta | Pantalla | Qué hace |
| --- | --- | --- |
| `/` | Lista | Muestra los primeros 20 Pokémon (1, 2 o 3 columnas según el ancho de la pantalla) |
| `/pokemon/[name]` | Detalle | Muestra imagen, tipos, altura, peso y estadísticas del Pokémon |

## Estructura

```
app/
  _layout.tsx          navegación (Stack)
  index.tsx            lista
  pokemon/[name].tsx   detalle
hooks/
  usePokemonList.ts    pide la lista a la API
  usePokemonDetail.ts  pide el detalle a la API
types/
  pokemon.ts           interfaces de TypeScript
```

## Cómo correrla

```bash
npm install
npx expo start
```

Luego presiona `a` (emulador Android), `w` (navegador) o escanea el QR con Expo Go.
