# EE6893-Final-Project
## Generating Podcast Summaries with State-of-the-Art Language Models

### Project Goal
Automatic summarization of Podcast is a recent topic of research and interest. Existing NLP summary relies heavily on models trained on well-edited news or book corpus, whereas podcasts are longer, more conversational and less succinct. This project presents a process of compiling a Podcasts dataset, transcribing the audio file to text corpus, and compares GPT2, BERT and BART's capability to create summaries on podcast corpus.

### Files Included
`RSS Pull and Save.ipynb` 
- Pull mp3 files froom RSS feed provided, convert to .wav and upload to GCP storage
- Pull file from GCP storage, use GCP speech-to-text API to transcribe the file, and upload back to GCP storage

`Language Summary.ipynb`
- Pull transcripts from GCP storage and preprosses to pass through transformers
- Test performance of GCP2, BERT and BART on text summarization
