# Tihu Persia Dictionary

Tihu-dict is a pronouncing dictionary of Persian, suitable for uses in speech technology.

We welcome input from users. If you have new words with pronunciation tags, we would appreciate it if you could send these additions and corrections to mostafa.sedaghat@gmail.com for consideration in a subsequent version.

## Running G2P

This repository has a pre-trained model in Persian Language for [Sequence-to-Sequence G2P toolkit](https://github.com/cmusphinx/g2p-seq2seq). Please check the release page to download pre-trained models.
Unpack the model after download. The model is trained on [Tihu dictionary](./tihu.demo.dict).

```
wget -O g2p-seq2seq-tihudict.tar.gz https://github.com/tihu-nlp/tihudict/releases/download/v2.0/g2p-seq2seq-tihudict-model-2.0.tar.gz
tar xf g2p-seq2seq-tihudict.tar.gz
```

The easiest way to check how the tool works is to run it the interactive mode and type the words

```
$ g2p-seq2seq --interactive --model_dir model_folder_path
...
> سلام
...
Pronunciations: [s a l A m]
...
>
```

### Word Error rate
WER: 0.136, Accuracy: 0.864

## Supporting Tihu
If you like this project, please [donate](http://lilak-project.com/donate.php) or consider becoming a patron:

[![Become a patron](https://c5.patreon.com/external/logo/become_a_patron_button.png)](https://patreon.com/b00f)

## License
Tihu is published under GNU General Public License. You may freely use, reproduce, modify or distribute it. If you think lilak is useful please support it.

