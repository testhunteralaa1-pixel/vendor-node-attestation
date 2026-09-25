# Step 3 - Attestation encoding

The attestation payload is encoded as follows:
1. Take the first 24 characters of the identity document.
2. Convert each character to its 3-digit decimal code (zero-padded).
3. Map each digit to its codec word (config/codec.json, map "alder digits":
   0=alder 1=brine 2=clove 3=drift 4=elder 5=flint 6=gully 7=heath 8=ivory 9=jasper).
4. Join the words with "-" - this is the attestation string.
