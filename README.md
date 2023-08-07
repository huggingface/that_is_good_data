# That is good data

Did you ever have the frustrating experience of looking at the evaluation results of your NLP model, and realising that some of your model mistakes are in fact mistakes in the evaluation data?
You are not the only one.
In fact, you are likely not even the only one who observed that particular mistake in the data!
**Many people discover mistakes in commonly used evaluation datasets, but there is no real protocol to report and correct those mistakes** -- until now.
In this repository, we provide a venue to make sure that mistakes in evaluation datasets are recorded and eventually corrected (depending on the place of the data, of course) and -- importantly -- that they are visible to future researchers using datasets, in one place.

Go directly to the list of recorded [issues with individual sample](sample_issues.md) or the reported [entire dataset issues](dataset_issues.md).

## Table of contents
- [What kind of issues can I report?](https://github.com/huggingface/that_is_good_data#what-kind-of-issues-can-i-report)
- [How do I report issues?](https://github.com/huggingface/that_is_good_data#how-do-i-report-issues-with-evaluation-datasets)
    - [Reporting issues with individual examples](https://github.com/huggingface/that_is_good_data#reporting-issues-with-individual-examples-in-evaluation-datasets)
    - [Reporting entire dataset issues](https://github.com/huggingface/that_is_good_data#reporting-entire-dataset-issues)
- [Helping out](https://github.com/huggingface/that_is_good_data#helping-out)


## What kind of issues can I report?
At the moment, we keep track of two types of dataset issues:
- **Issues with individual examples** (e.g. the input sentence is ambiguous wrt label, the input is incomprehensible, the label is incorrect or it is not clear why it should be prefered over another label). While we first start with collecting these examples, our eventual aim is to make sure they also get *corrected* or removed from the dataset in question.
- Known (and published) issues/problems that pertain to datasets as a whole (e.g. strong correlation between labels and lexical items, strong contamination in commonly used training corpora). Depending on what a dataset is used for, biases may not always be problematic, but it is nevertheless always good to be aware of.

For the moment, we collect individual mistakes in a series of spreadsheets, that can be found on the [individual sample issues](sample_issues.md) page. 
If a dataset is not listed on this page this implies no errors have been reported for it yet (in this repository).

Issues with entire datasets are recorded on the [entire dataset issues page](dataset_issues.md) in this repository. 
If a dataset is not listed on this page, it means we have not received any input on biases in these datasets.

## How do I report issues with evaluation datasets?
For the time being, there are two options for contributing isues/mistakes/biases to this dataset:
- Create an issue on this repository
- Fill in [this form](https://forms.gle/CjhzTsRVQCVghHgC6)

Below, you can find what information you should provide, depending on what kind of issue your contribution reports.

### Reporting issues with individual examples in evaluation datasets
To report a mistake in a dataset, fill out [this form](https://forms.gle/CjhzTsRVQCVghHgC6), or create an issue on this repository with the following information:
- The dataset name
- A link to the source of the dataset, with a commit sha (or other kind of time stamp). If the dataset is available on [HuggingFace datasets](https://huggingface.co/datasets), provide the HuggingFace link.
- The index of the example that contains a mistake -- if the dataset is available on HuggingFace, you can directly link to the example (e.g. [https://huggingface.co/datasets/cais/mmlu/viewer/professional_psychology/validation?row=8])
- The example itself or the relevant parts of the example (if there is a lot of text), written out 
- A description of the issue with the example
- For multilingual datasets: Which language(s) are affected
- Whether and how the issue could be fixed (optional)
- Whether you'd like to receive public credit for detecting the mistake in this repository

We will review reported issues on a rolling basis and incorporate them in the repository, crediting you if you wish.
If you found these issues by checking a larger batch, we welcome it if you also provide the number of examples you checked and/or the id's of the examples you *didn't* find any issues with.

If you'd like to report more than one mistake but (understandably) don't feel like filing multiple issues or filling out the form multiple times, please reach out to us at <that-is-good-data@googlegroups.com>.
You can, for instance, provide us a spreadsheet that contains the information above for all examples you'd like to report.

### Reporting entire dataset issues

Also biases or issues with entire datasets beyond individual examples can be submitted through github issues, or through the [form](https://forms.gle/CjhzTsRVQCVghHgC6) linked above.
Because we cannot confirm these biases ourselves, we require that there is peer-reviewed paper that exposes the bias.

If you'd like to report an issue with a dataset, please report:
- The dataset name
- A link to the source of the dataset, with a commit sha (or other kind of time stamp). If the dataset is available on [HuggingFace datasets](https://huggingface.co/datasets), provide the HuggingFace link.
- A short description of the issue
- A link to the publication that exposes the issue
- Whether and how the issue could be fixed (optional)
- Whether you'd like to receive public credit for detecting the mistake in this repository

## Helping out
Interested in helping out?
Apart from reporting issues with datasets, we are also looking for people that can help out with validating reported issues, especially for languages that we cannot judge ourselves!
For more information, check the [contributions file](CONTRIBUTING.md)

## Initiators of this initiative
This initiative was set up by [Dieuwke Hupkes](https://dieuwkehupkes.nl), [Xenia Ohmer](https://xeniaohmer.github.io/), [Thomas Wolf](https://thomwolf.io/) and [Adina Williams](https://scholar.google.com/citations?user=MUtbKt0AAAAJ&hl=en).
