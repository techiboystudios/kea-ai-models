# Kea on-device AI packages

Public release assets for Kea Android. Kea downloads these only after the user selects Download in Settings → AI packages. Files are stored in Kea private app storage. Model inference stays on the phone; package requests do not include screen content, search queries or saved items.

## Release `ai-data-v1.0.0`

| Asset | Purpose | Size | SHA-256 | License / attribution |
|---|---|---:|---|---|
| `board_encoder.tflite` | MediaPipe Universal Sentence Encoder QA text-embedding model for local semantic matching | 6,120,274 bytes | `89ad3c74175dd8caa398cc22b657296d94302d20c525c12b58b29420f7249749` | Apache-2.0; Google Universal Sentence Encoder |
| `dictionary.db` | Open English WordNet 2025 SQLite data for offline English word lookup | 15,421,440 bytes | `2f786ac8b9e9170d692e0d39869c5fad4a529dcc44228dc8ed191be69d591a05` | CC BY 4.0; Open English WordNet |

The semantic encoder produces text embeddings; it does not generate text or inspect image pixels. Dictionary lookups are English only.

Google ML Kit OCR, language identification, face detection and subject segmentation packages are delivered separately by Google Play services. Translation language packs are downloaded from Google when selected.

## Attribution and licenses

- Universal Sentence Encoder QA model: Apache License 2.0.
- Open English WordNet: Creative Commons Attribution 4.0 International. Source: https://github.com/globalwordnet/english-wordnet
