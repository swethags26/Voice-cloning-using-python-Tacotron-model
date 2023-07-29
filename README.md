# Text-to-Speech (TTS) using Tacotron

This project implements a Text-to-Speech (TTS) system based on the Tacotron model. The Tacotron model is a sequence-to-sequence architecture that can generate mel-spectrograms from input text, which can then be converted into high-quality speech using a vocoder like WaveRNN. The project includes data preprocessing, model definition, training, and evaluation tools.

## Prerequisites

- Python 3.x
- PyTorch
- librosa
- soundfile
- lws

You can install the required dependencies using the following command:

## Project Structure

- `synthesizer/`: Contains the Tacotron model definition and training code.
- `vocoder/`: Contains the WaveRNN vocoder code (not included in this README).
- `datasets/`: Put your training dataset in this directory.
- `metadata.csv`: The metadata file containing the information about the training data.
- `tacotron_hparams.py`: Configuration file for model hyperparameters.
- `train_tacotron.py`: The main script for training the Tacotron model.
- `synthesize.py`: Use this script to synthesize speech from trained Tacotron model.
- `eval_tacotron.py`: Evaluate the Tacotron model performance.

## Usage

1. Prepare your training dataset and place it in the `datasets/` directory. Create a `metadata.csv` file containing relevant information about the training data.
2. Set the desired hyperparameters in `tacotron_hparams.py`.
3. Train the Tacotron model using `train_tacotron.py`.
4. Optionally, evaluate the model using `eval_tacotron.py`.
5. Synthesize speech from trained model using `synthesize.py`.

## Acknowledgments

This project is based on the Tacotron model implementation by Keith Ito (https://github.com/keithito/tacotron).

## License

This project is licensed under the MIT License - see the LICENSE file for details.
