# ACM-Compute-Poster---2018

#### Requirements : ####
* Tensorflow
* Python 2.7+

#### Files : ####
* vocab.txt --> It consists of words and their ocurrences.
* model.py --> This class is responsible for loading the graph, creating image embeddings, and running an inference step on the model.
* vocabulary.py --> This class is responsible for mapping words to ids.
* create_caption.py --> This class is used for generating captions
* loading_model.py --> This class loads the VIAssistant.pb model and use it with the above caption generator to create sentences. These sentences will be printed along with their log probability.

#### Execution : ####
```
python loading_model.py --model_path VIAssistant.pb --input_files image.jpg --vocab_file vocab.txt
```

```
--model_path --> Model graph def path 
--input_files --> File pattern or comma-separated list of file patterns of image files. 
--vocab_file --> Text file containing the vocabulary.
```
