---
notes: |
  - prepublish
  - who knows
  - history of the only part
  - builds and includes dist (if you allow it in you npm ignore file)
  - consume as npm or use another one weird trick
  - whoo knows about unpkg

  “prepublishOnly”: “rm -rf dist && npm run build”

  Who here knows what `prepublishonly` actually does? It’s a neat trick that makes sure that you run this whenever you’re in the process of publishing your package to npm. The reason it’s called “prepublishonly” and not just “prepublish” is because of some legacy npm issues where that hook used to also be called on install which is just silly. I don’t think it’s a problem for `npm@7` any more but I guess it’s force of habit that I still use this one.

  now when you publish your repo to npm it also runs `npm run build` which compiles your css into a vendor.css in the dist/asseets folder.

  So you can either consume this package now using npm if you already have an npm based pipeline, or you could just be old school and link that file directly in your html using another “one weird trick”. How many people here know about unpkg?
---

# prepublish

![Chris](/images/prepublish.webp)
