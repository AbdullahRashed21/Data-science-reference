Today we'll practice building recurrent neural networks and applying transfer learning with text data. 
We'll use a kaggle dataset of sentences from 3 different authors, with the model goal being to classify the author using only the sentence.

1) Start by loading in the data (`author_data.csv` in this directory) and preparing it for modeling, including a train-test split.

You can modify the code block given below, adding in the appropriate steps specified by the ### comments.
In particular, you will need to add the code to **create and fit a tokenizer** and to **convert documents to padded sequences**.

```

from tensorflow.keras.preprocessing.text import Tokenizer
from tensorflow.keras.preprocessing.sequence import pad_sequences
from tensorflow.sklearn.model_selection import train_test_split
from tensorflow.keras.utils import to_categorical 

### DEFINE Tokenizer with max vocabulary 15k, FIT on all text (author_df.text)

# standard train/val split
X_train, X_test, y_train, y_test = train_test_split(author_df.text, author_df.author, 
                                                    test_size=0.2, random_state = 42)

# multiclass output formatting
y_train_cat = to_categorical(y_train)

### CONVERT X_train to token sequences 
### PAD X_train to length 50

### CONVERT X_test to token sequences
### PAD X_test to length 50

```

2) Use keras to build a simple RNN model that converts input sequences to custom-trained word embedding (dim ~40) sequences
before passing these sequences to a recurrent layer. With a simple model, it should be possible to exceed 80% accuracy on train, validation, and test.

You may use the sequence lesson material as a reference for this and the next steps.

3) Use keras to build a transfer learning RNN for this problem: replace custom-trained embeddings with pre-trained embeddings.

This step will require you to initialize and fill an `embedding_matrix` to pass to the keras embedding layer --
see lesson material for an example. If you don't already have pre-trained embeddings saved locally, you can download and use the google news
vectors here: [GoogleNews-vectors-negative300.bin.gz](https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/edit).

Prioritize getting a functioning, trainable model for this step. You may be dissapointed by the results! 

4) (Extension) if time permits, try to improve your model by using a **hybrid approach**: combining pre-trained embeddings with embeddings learned on the fly. You will want to define 2 embedding layers (as in steps 2 and 3), and concatenate them using the keras `Concatenate` layer (don't hesitate to look up the documentation!)


