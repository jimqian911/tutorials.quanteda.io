---
title: "quanteda tutorials"
chapter: false
---
# Quanteda tutorials

{{% author %}}By [Kohei Watanabe](http://koheiw.net) and [Stefan Müller](http://muellerstefan.net){{% /author %}} 

This website contains a step-by-step introduction to quantitative text analysis using **quanteda**. The chapters cover a brief introduction to the statistical programming language R, how to import text data, basic operations of **quanteda**, how to construct a corpus, tokens objects, a document-feature matrix, and how to conduct advanced operations. The final chapter deals with text scaling (e.g., Wordscores, Wordfish, correspondence analysis), document classification using Naive Bayes and topic models.

The six chapters consist of over 30 sections. If you click on the name of a chapter on the left-hand side of this page, the sections will pop up. You can also use the "Search" field in the top-left corner to look up the occurrence of certain terms or R functions covered in the tutorials. 

This website is created for workshops held by the **quanteda** team and for users who look for a comprehensible step-by-step introduction to text analysis using R. We have also created several additional useful [resources](https://quanteda.io), such as vignettes, replications, a cheatsheet and a comparison to other text analysis packages (in terms of [functions](https://quanteda.io/articles/pkgdown/comparison.html) to get you started. 

You can not only see the R commands but execute them yourself if you [download the source code of this website](https://github.com/quanteda/tutorials.quanteda.io/archive/master.zip) from the [Github repository](https://github.com/quanteda/tutorials.quanteda.io). You should unzip the files on your machine and click `quanteda_tutorials.Rproj` to open RStudio. Executable R commands are in the `.Rmarkdown` files under the `content` folder.

Contributions in the form of feedback, comments, code, and bug reports are most welcome. If you have questions on how to use **quanteda**, please post them to [the quanteda channel on StackOverflow](https://stackoverflow.com/questions/tagged/quanteda). If you find a bug, please report it to the [quanteda issues](https://github.com/quanteda/quanteda/issues). *We prefer these platforms to emails in communicating with our users* because the records will help other users who have similar problems.

{{% notice note %}}
Examples in this tutorial are written for **quanteda** version 1.4.0. Please check if you have the same version installed by a command `packageVersion("quanteda")`. 
{{% /notice %}}

{{% notice info %}}
If you use this website in courses or publications, please cite it as: Watanabe, Kohei and Stefan Müller. 2019. *Quanteda Tutorials*. https://tutorials.quanteda.io.
{{% /notice %}}
