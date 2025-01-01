# Tamil-LM


This repository contains a custom tokenizer designed specifically for the Tamil language, along with a vast collection of Tamil resources, including literary texts and other datasets. The tokenizer is built to handle both Unigram and BPE (Byte Pair Encoding) tokenization methods, optimized for processing and understanding Tamil texts.

The goal is to create a comprehensive collection of Tamil resources for various purposes, including research, general use, and more. While the tokenizer is being developed to support TamilBERT, the TamilBERT development is separate, and the community is encouraged to explore and try out new ideas, contribute to the tokenizer, and experiment with Tamil language models for different applications and use cases.

---
## Contents

- **Tokenizers**: 
  - Unigram Tokenizer (12,000 vocab)
  - BPE (Byte Pair Encoding) Tokenizer (55,000 vocab)
- **Tamil Text Dataset**: A collection of Tamil literary texts, including data from Tamil Sangam and other Tamil scriptures.(it's all mixed together will take some time to preprocess and publish, contributions are welcomed.)

---

## Sources

- **Literary Texts**:

  - *நாலாயிர திவ்ய பிரபந்தம் / திருப்பல்லாண்டு*
  - *நாலாயிர திவ்ய பிரபந்தம் / திருப்பாவை*
  - *நாலாயிர திவ்ய பிரபந்தம் / நாச்சியார் திருமொழி*
  - *திருவாசகம் (1-10)*
  - *ஐங்குறுநூறு*
  - *சிறுபாணாற்றுப்படை*
  - *குறுந்தொகை*
  - *புறநானூறு*
---

## Usage

```bash
git clone https://github.com/your-username/tamil-tokenizer.git
cd tamil-tokenizer
```
``` python
from transformers import PreTrainedTokenizerFast
tokenizer = PreTrainedTokenizerFast.from_pretrained('/BPE_Tokenizer', model_max_length=512) ## Use Unigram_Tokenizer to use unigram tokenizer
tokens = tokenizer.tokenize("வணக்கம் உலகம்")
print(tokens)
```

## Contributing

If you wish to contribute to the development of the tokenizer or the dataset, feel free to open an issue or pull request. Contributions are welcome!
