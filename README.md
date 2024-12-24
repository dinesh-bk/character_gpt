# CharacterGPT: A Custom GPT Model for Character-Level Tokenization

This project focuses on building a custom GPT model that operates on character-level tokenization. The notebook provides tools for creating a tokenizer, building the dataset, and training a GPT-like model from scratch, making it suitable for tasks like generating text at a character level. Below is an overview of the repository's structure and functionality.

---

## Key Features
- **Custom Character-Level Tokenizer**: A tokenizer tailored for character-based operations, complete with special tokens and functionality for encoding and decoding.
- **Dataset Handling**: Efficient preparation and handling of datasets for training.
- **Training Pipeline**: Code for defining and training a transformer-based GPT model.

---

## Structure of the Notebook

### 1. **Dependencies and Imports**
The project uses the following libraries:
- Transformers
- PyTorch
- NumPy
- TQDM

### 2. **Tokenizer Creation**
The `CharacterTokenizer` class is defined to tokenize text at the character level. Key functionalities include:
- Special token handling (e.g., `[BOS]`, `[EOS]`, `[PAD]`)
- Vocabulary management
- Serialization and deserialization for saving and loading pre-trained tokenizers.

### 3. **Dataset Preparation**
The notebook demonstrates how to structure and process datasets for character-level tokenization, ensuring compatibility with the tokenizer and model.

### 4. **Model Training**
A training pipeline is set up using PyTorch:
- Definition of a GPT-like model architecture.
- Efficient training loops using AdamW optimizer.
- Metrics for monitoring training progress.

---

## Installation and Setup
1. Clone this repository.
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Install the required dependencies.
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook using Jupyter or any compatible environment.

---

## Usage
1. Modify the `characters` variable in the tokenizer class to define your character set.
2. Prepare your dataset by following the instructions in the "Dataset Preparation" section.
3. Execute the notebook cells sequentially to train the model.

---

## Outputs
- **Tokenizer**: Saved in the `tokenizer_config.json` file.
- **Trained Model**: Checkpoints saved periodically during training.

---

## Future Work
- Support for additional special tokens.
- Implementation of evaluation metrics specific to character-level tasks.
- Fine-tuning on specific tasks such as name generation, text correction, etc.

---

## License
This project is licensed under the MIT License. See the LICENSE file for details.

---

## Acknowledgments
- [Hugging Face Transformers Library](https://huggingface.co/transformers/)
- PyTorch Community

