# Enchant | NoobMaster — Write-up

**Description:**  
Description: I was playing minecraft, and found this strange enchantment on the enchantment table. Can you figure out what it is? Wrap the flag in `scriptCTF{}`.
There was an attachment, enc.txt.

`enc.txt:`  
ᒲ╎リᒷᓵ∷ᔑ⎓ℸ ̣ ╎ᓭ⎓⚍リ

---

## Walkthrough

The symbols in the provided text match the **Standard Galactic Alphabet (SGA)** — the fictional runic script used on Minecraft enchantment tables.

To decode it, I mapped each glyph to its SGA counterpart. Transliteration gave the plaintext:

minecraftisfun

Nothing tricky, no XOR, no ciphers — just straight SGA.

---

## Final Flag
### scriptCTF{minecraftisfun}
