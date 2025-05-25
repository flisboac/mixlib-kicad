The file naming scheme is unaltered from TI's own, with the addition
of the `TI_` prefix to indicate the vendor (Texas Instruments), and
change to uppercase on the file name's stem. The suffix will always
be `.cir` (changed from the original `.lib` suffix).

Format:

{PART_NUMBER}{QUALIFIER}{VOLTAGE}_{MODEL_TYPE}.cir

Where:

- PART_NUMBER is just the model's part number.
  If the P/N contains a dash, TI replaces that with an underscore.
  For example: "LM4040-N" becomes "LM4040_N"
- QUALIFIER is just a letter. I'm unsure what it indicates;
  it doesn't seem like it's part of the P/N, but at the very
  least it serves as a separator between the P/N and the
  nominal reference voltage.
- VOLTAGE is just the nominal reference voltage, with the decimal
  point replaced with the letter "P"; e.g. "4.096V" becomes "4P096".
- MODEL_TYPE is the variant of the model.
  It will most likely be just TRANS, to indicate the model was created
  for use in transient analysis.
