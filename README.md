# About

**[LocalShiny][host]** is designed to help with the data security problem, i.e. when an organization, who has some fairly stringent guidelines around data privacy and related issues, does not want to share their data with a third party. It automates the process of installing shiny apps and avoids the problem referenced above by running apps in your own machine.

**LocalShiny** consists of three components, `LocalShiny Web`, `LocalShiny R package` and `LocalShiny Software`. LocalShiny Web is an online service for hosting Shiny apps in the cloud. Developers, who want to share Shiny web applications built in R, use the LocalShiny R package to create the clones of your applications and then deploy them in the cloud. Users use LocalShiny app to reproduce Shiny web applications on their own computer machine. The client installs R and Shiny apps, and runs apps with only one click.

## The Origin of LocalShiny

A typical statistical research starts from identifying the research problem. Then, novel methods are developed to tackle the problem. Theoretical properties of the proposed methods are derived. Often, numerical studies are conducted to evaluate the performance of the methods. Finally, the results are reported in peer-reviewed articles and published in statistical journals.

With the ever increasing R community, this typical statistical research life cycle has been extended by developing R software packages and distributing (e.g., through the Comprehensive R Archive Network) the method among R users, mostly peer statisticians. Recently, R Shiny has become popular to further extend this life cycle by developing web-based user-friendly software, so that non-statisticians can easily access to the novel methods.

However, the distribution of R Shiny applications requires setting up specific web servers, which can be prohibitive for statisticians. On the other hand, for users such as clinicians, web-based software hosted by public web servers can be infeasible since such web servers may not comply with the data privacy constraints.

We are developing an all-in-one solution for statisticians to distribute their R Shiny applications to users. The solution comprises three components. First, we will develop an R package, LocalShiny, that can automatically compress the R Shiny application files and its running environment settings into an installation file. Second, the installation files will be uploaded (by LocalShin) to STAPP, an online repository of such installation files. Third, we will develop a Qt-based cross-platform stand-alone software that can download a specific installation file from STAPP, and call out and run the R Shiny application from the installation file. As the final product, the all-in-one solution will allow statisticians to upload their R Shiny applications to STAPP by a one-line command, and allow users to interactively download, install and run an R Shiny application from their local computers. This solution will significantly enhance the work-flow efficiency for statisticians to distribute their methods to users.

## Software/Package

| Name | Source | Description |
| :--------------------------------- | :-------------------------- | :--------------------------------------------------------------- |
| [R](https://www.r-project.org)     | https://www.r-project.org   | LocalShiny R package built with R depends on [renv](https://rstudio.github.io/renv/) and [RCrul](https://CRAN.R-project.org/package=RCurl) |
| [Shiny](https://shiny.rstudio.com) | https://shiny.rstudio.com   | LocalShiny assists statisticians to distribute R Shiny applications to users |
| [Python](https://www.python.org/)  | https://www.python.org/     | LocalShiny Web built with Python packages on [Pypi](https://pypi.org/) and [Flask](https://flask.palletsprojects.com/) |
| [Qt](https://www.qt.io)           | https://www.qt.io           | LocalShiny Software is Qt-based cross-platform stand-alone software |

<!-- ## About Team

LocalShiny is developed and maintained by Dalian University of Technology and Johns Hopkins University.

<img src="./images/dut.png" alt="dut" style="zoom:100%;" />		<img src="./images/jhu.png" alt="jhu" title="JHU" style="zoom:100%;" /> -->

## Feedback

You can view the source code of [LocalShiny R package ](https://github.com/localshiny/localshiny) and [LocalShiny Software](https://github.com/localshiny/QT) on [LocalShiny Github](https://github.com/localshiny).

Should you have questions about how LocalShiny Web works, or how you can get your apps to run well via LocalShiny Software, or should you have news tip, suggestion, idea or think something is missing on LocalShiny, contact **localshiny@gmail.com**.

--------------------------
[host]:http://www.findn.cn:5000 "LocalShiny"