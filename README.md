# Dataset Indonesian LER

This repository contains the dataset used in our undergraduate thesis. The dataset contains 993 annotated court decission document. The document was taken from [The website of Supreme Court of Indonesia](https://decision3.mahkamahagung.go.id/). the documents have also been tokenized and cleaned. The data is stored using JSONL format with fields as follows:

```json
{
	"text" : "Word-splitted text",
	"text-tags" : "IOB formatted label"
}
```

## Here's one sentence from the dataset:

```json
{
	"text": ["PUTUSAN", ".", "NOMOR", ":", "1974", "/", "Pid", ".", "Sus", "/", "2012", "/", "PN", ".", "JKT", ".", "BAR", ".", "DEMI", "KEADILAN", "BERDASARKAN", "KETUHANAN", "YANG", "MAHA", "ESA", "."],
	"text-tags": ["O", "O", "O", "O", "B-putusan", "I-putusan", "I-putusan", "I-putusan", "I-putusan", "I-putusan", "I-putusan", "I-putusan", "I-putusan", "I-putusan", "I-putusan", "I-putusan", "I-putusan", "I-putusan", "O", "O", "O", "O", "O", "O", "O", "O"]
}
```

We also provided the metadata of the data also in JSONL format. The metadata provided are:

```json
{
	"verdict": "The type of verdict given in the document (guilty, bebas, or lepas)",
    "indictment": "The type of indictment presented to the court (Tunggal, subsider, komul, alternatif, kombinasi, or gabungan)", 
    "lawyer": "whether the defendant has a lawyer present", 
    "id": "the internal id of the document", 
    "owner": "the person who annotate the document"
}
```

We also provide the data we used in each split in CSV format.

## Reference
Please cite the following paper if you use this dataset:

WIP

## Contact
**naradhipabhary27 [at] gmail.com**
