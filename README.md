# fortnite-cosmetic-list
Scraped JSON list of all fortnite cosmetics and their properties from fortnite.gg.

## Object example
```
{
  "Id": "CID_959_Athena_Commando_M_Corny",
  "FortniteGgId": "16",
  "Name": "Cobb",
  "Description": "Shake off that husk and grab some butter.",
  "PriceVbucks": 1200,
  "Season": "c2s4",
  "Source": 1,
  "Rarity": 3,
  "Type": 1,
  "Set": "Kernel Commando",
  "Release": "2020-11-25T00:00:00",
  "LastSeen": "2023-10-03T00:00:00",
  "Styles": [
    "DEFAULT",
    "NON-REACTIVE",
    "FULL POP"
  ],
  "Tags": [
    1,
    2
  ]
}
```

Empty or null values are ommited. Uses .NET's [UnsafeRelaxedJsonEscaping](https://learn.microsoft.com/en-us/dotnet/api/system.text.encodings.web.javascriptencoder.unsaferelaxedjsonescaping?view=net-8.0#system-text-encodings-web-javascriptencoder-unsaferelaxedjsonescaping).

## Properties
```
#### Id (string)
#### FortniteGgId (string) - Item ID used by fortnite.gg
#### Name (string)
#### Description (string)
#### PriceVbucks (string)
#### PriceUsd (string)
#### Season (string) - Cosmetic's release season, format: c[1-9]s([1-9]|X|OG)
#### Source (enum)
- Unknown = 0
- Shop
- Battle Pass
- Crew
- Challenges
- Exclusives
- Packs
#### SourceDescription (string) - Explanation on obtainability
#### Rarity (enum)
- Unknown = 0
- Common
- Uncommon
- Rare
- Epic
- Legendary
- McLaren
- Lamborghini
- Star Wars Series
- Slurp Series
- Shadow Series
- Marvel Series
- Lava Series
- Icon Series
- Gaming Legends Series
- Frozen Series
- DC Series
- Dark Series
#### Type (enum)
- Unknown = 0
- Outfit
- Backpack
- Wrap
- Pickaxe
- Bundle
- Emote
- Glider
- Loading Screen
- Music
- Contrail
- Spray
- Emoji
- Toy
- Banner
- Build
- Decor
- Car
- Decal
- Wheels
- Trail
- Boost
- Jamtrack
- Guitar
- Bass
- Drums
- Keytar
- Microphone
- Aura
#### Set (string)
#### Release (DateTime)
#### LastSeen (DateTime)
#### Styles (string[]) - Just a list of all (=listed on fortnite.gg) style names
#### Tags (enum[])
- Forged = 0
- Styles         // (Selectable Styles || Unlockable Styles)
- Reactive
- Traversal
- Built-in
- Synced
- Animated
- Transformation
- Enlightened
```
