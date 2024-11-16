# es335-24-fall-assignment-4
# Instructions to set up the project locally
```bash
python3 -m venv env
```
Activating the environment on Windows:
```bash
env\Scripts\activate
```
Activating the environment on MacOS/Linux:
```bash
source env/bin/activate
```
Installing dependencies:
```bash
pip3 install -r requirements.txt
```

# Solutions

## Question-1: 
[`./question_1.ipynb`](./question_1.ipynb)
### Are the results as expected? Why or why not?
Yes, the results are mostly expected but certain better and larger models show unexpected behaviour with poor performance. This is due to training at less number of epochs.
### Does data augmentation help? Why or why not?
Data augmentation involves applying random transformations (like rotations, flips, cropping, and color changes) to the training images, which effectively increases the diversity of data available to the model.

**Increases Variability:** By exposing the model to slightly altered versions of the images, data augmentation helps the model learn more robust features, making it less likely to overfit to specific details of the training images.

**Improves Generalization:** The transformations simulate real-world variations, which makes the model more adaptable to variations in new data.

**Reduces Overfitting:** In cases of small datasets, overfitting is a common problem. Data augmentation helps by artificially enlarging the dataset and reducing the model’s dependence on specific patterns, improving generalization to unseen data.

### Does it matter how many epochs you fine-tune the model? Why or why not?
Fine-tuning for too few epochs may result in underfitting, where the model hasn’t yet learned enough about the specific features of the new dataset. Fine-tuning for too many epochs may lead to overfitting, where the model starts to "memorize" the fine-tuning dataset instead of learning generalizable features.

**Learning Rate and Pre-trained Weights:** Since fine-tuning generally starts from pre-trained weights, the learning rate and number of epochs need careful adjustment to avoid "forgetting" useful, general features learned from the pre-training dataset.

### Are there any particular images that the model is confused about? Why or why not?
Yes, there are many images of black ducks that the model predicts as magpies. This confusion may be due to the similarity in the color of the two birds, especially when the black duck is in a similar pose to the magpie. When a magpie is in flight, its body shape can appear more rounded, which could be mistaken for a duck, especially if the distinctive tail feathers are not clearly visible.

## Question-2: 
[`./question_2.ipynb`](./question_2.ipynb)


# Questions
## Question-1 [6 Marks]






