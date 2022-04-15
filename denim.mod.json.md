# THE FUCKING MARKDOWN
Aw yea baby, boutta make a Denim mod.
But wait, how do you do the dew?
I gotchu fam!
    
## `schemaSpaceVersion`
| Type   | Required |
|--------|----------|
| int    | True     |

Basically this tells the loader the version of the schemas, you know? The schemas, only something an idiot wouldn't know.

## `id`
| Type      | Required |
|-----------|----------|
| boolean[] | True     |

The ID for your mod, so that it can go to a bar and get some if you know what I'm sayin'
It has to be typed out in ASCII, but with booleans.
So like if a letter is 01100100, you have to do
`false, true, true, false, false, true, false, false`

## `version`
| Type   | Required |
|--------|----------|
| String | True     |

The version bro

## `description`
| Type   | Required |
|--------|----------|
| int    | False    |

This describes what kind of mod your mod is to Denim, so for example
0 is loader
1 is an API
2 is gbro's secret lolicon Reddit account
3 is magic
4 is something I made when I was high on weed
And so on, obvious stuff dude.

## `author`
| Type   | Required |
|--------|----------|
| String | False    |

The person who wrote the mod.

## `otherAuthor`
| Type   | Required |
|--------|----------|
| String | False    |

The other person who wrote the mod.
The spec only covers two because fuck you third wheel that's why.
Sharon was supposed to be mine but you fucking took her away from me you piece of shit Jason

![Fak](https://cdn.discordapp.com/attachments/894994408733286451/964372007473008650/VignePleadHDfacecrop.png)


## `contact`
| Type   | Required |
|--------|----------|
| Object | False    |

A bunch of shit telling people how to contact you.
Inside you have the ability to put your email, phone number, home address, and MinecraftForums username.

## `canYouDrive`
| Type   | Required |
|--------|----------|
| String | False    |

If you don't put this it's automatically assumed that you can't drive bro

#### The `icon` field
| Type          | Required |
|---------------|----------|
| Object        | False    |

The icon for your mod, we have a few options for it.
The possible values for "type" are
`google-images`, `bing-haha-nobody-uses-bing`, `pixiv-probably-porn`, `file` (The normal one that gets a PNG inside the mod), and `youtube-thumbnail` 

The value for "value" is what would be fed into the type.

## `mixins`
| Type   | Required |
|--------|----------|
| String | False    |

Basically this is what calls the mixin config, or mixin config directory if you want that.


## `environment`
| Type   | Required |
|--------|----------|
| String | False    |

Uhh the planet you're on I think

## `cum`
| Type   | Required |
|--------|----------|
| Object | True     |

The most important bit.
It doesn't do anything for the mod, but Denim won't start without it.
In order to be valid, you need the value "theCumPassword" inside the holy Cum Block to be set to "C U M".

## Example
An example denim.mod.json:
```json
{
  "schemaSpaceVersion": 1,
  "id": [
    false, true, true, false, false, true, false, false,
    false, true, true, false, false, true, false, true,
    false, true, true, false, true, true, true, false,
    false, true, true, false, true, false, false, true,
    false, true, true, false, true, true, false, true
  ],
  "version": "0.17.0",
  "description": 4,
  "environment": "earth",
  "author": "PseudoDistant",
  "otherAuthor": "TheSpecOnlyCoversTwoAuthorsFuckYou",
  "contact": {
    "phoneNumber": "867-5309",
    "email": "definitelyrealemail@hotmail.com",
    "minecraftForumsUsername": "PseudoDistant"
  },
  "canYouDrive": "Apache-2.0",
  "icon": {
    "type": "google-images",
    "value": "toaster png"
  },
  "mixins": "0110010001100101011011100110100101101101.mixins.json.d/",
  "cum": {
    "theCumPassword": "C U M"
  }
}
```

We pulled out mod dependency parsing because it's for pussies, just read the stacktrace. L
