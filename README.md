# WASSA2022 Track 2
****Emotion Classification at the essay-level

Took 7th place out of 14 teams.

We conducted many experiments with different approaches, but the main issue was fighting with imbalance across classes. Thus, we tried different available emotion datasets for the augmentation, it improved the scores by few hudredths, but none of them were similar to our data. We also expected to enhance the performance by combining some classes at first step (for instance, neutral, positive, negative emotions) and then train more specific classifiers to distinguish inside the obtained groups. Though it did not really work, as even with binary classification on the first step f-score was at max around 80 (which is not enough for the initial split).  All in all, the best model was an ensemble of 2 fine-tuned BERT-based models and fine-tuned T5 model, final prediction was formed by majority voting.

Contributions: 
- Zhenya Egorova - ML approaches, Confusion Matrix Analysis, BERT-based models, Final ensemble, experiments with some data transformations and combinations of several classes in order to form ensemble, .
- Nastya Chizhikova - Simple Perceptron approaches, LSTM and attention experiments, data augmentation, T5 model

