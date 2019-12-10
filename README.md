# NLP_summarization_toy_examples

The results of very simple summaries evaluated with different python libraries based on ROUGE metric

The libraries are:

a. java ROUGE 2.0 https://rxnlp.com/rouge-2-0/#.XdXcKuhKiUk (no stemming, no stop words removal and no synonyms dictionaries)

b. easy-rouge python https://pypi.org/project/easy-rouge/

c. rouge python https://github.com/pltrdy/rouge (the output and reference summary files must contain the same number of lines)

d. wrapper of ROUGE 1.5.5.pl on python (default configuration: -c 95 -2 -1 -U -r 1000 -n 4 -w 1.2 -a -m) intalled following tutorial from https://medium.com/@prabha88978/installation-working-process-of-rouge-1-5-5-6c0dfdca49e8 and https://ireneli.eu/2018/01/11/working-with-rouge-1-5-5-evaluation-metric-in-python/#more-1840, the original ROUGE 1.5.5.pl can be obtained in https://github.com/bheinzerling/pyrouge located in pyrouge folder

The folder "toy_example1" contains three variant of summaries:

a. plain text

b. contains some punctuation marks

c. the text is in one sentence format

The notebooks (.ipynb files) contains the python implementations (easy-rouge and rouge python, both run in colab) and in their cell output we can observe the ROUGE metric.

Original ROUGE 1.5.5.pl wrapper does not run in colab (something related to Permission denied: '/content/gdrive/My Drive/Codigos_doctorado_DUC2001/pyrouge-master_with_ROUGE155/tools/ROUGE-1.5.5/ROUGE-1.5.5.pl'). But, I installed locally in jupyter notebook. The ROUGE metric for each output summary is contained in numpy files (.npy) named ROUGE_2002_toy_example_simple (plain text), ROUGE_2002_toy_example_simple_punctuation (contains punctuation marks) and ROUGE_2002_toy_example_simple_one_line (the text is in one sentence format) for pyrouge library.

The output files from java ROUGE 2.0 are comma separated files (.csv).

--------------------------------------------------------------------------------------------------------------------------------------

The folder "toy example2" contains two documents to summarize and one gold standard. The first document has three sentences, the second has four sentences and the gold standard has four sentences. For this example I create four output summaries (located in "toy_example2_d1", "toy_example2_d2", "toy_example2_d3". "toy_example2_d4" folders), which contains the following:

a. The last two sentences from document one and document two

b. The sentences of both documents

c. The sentences from document one

d. The sentences from document two

The "toy_example2_model_summaries" folder contains the gold standard.

The notebooks (.ipynb files) contains the python implementations (easy-rouge and rouge python, both run in colab) and in their cell output we can observe the ROUGE metric.

The ROUGE metric for each output summary is contained in numpy files (.npy) named ROUGE_2002_toy_example2_d1, ROUGE_2002_toy_example2_d2, ROUGE_2002_toy_example2_d3 and ROUGE_2002_toy_example2_d4 for pyrouge library.

The output files from java ROUGE 2.0 are comma separated files (.csv).

----------------------------------------------------------------------------------------------------------------------------------------

