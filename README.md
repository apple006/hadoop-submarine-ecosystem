# hadoop-submarine-ecosystem

## Why need this repo?

As discussed with several Apache Hadoop® committers, we plan to work outside of the Apache infrastructure to allow ecosystem features to be hardened and improved without creating risk for Apache projects. Once feature(s) of this repo becomes stable, we will merge it back to Apache projects follow normal Apache feature merge process.

## Apache Hadoop Submarine Miscs

Apache Hadoop {Submarine} is the latest machine learning framework subproject in the Apache Hadoop 3.2 release. It allows Hadoop to support `Tensorflow`, `MXNet`,` Caffe`, `Spark`, etc. A variety of deep learning frameworks provide a full-featured system framework for machine learning algorithm development, distributed model training, model management, and model publishing, combined with hadoop's intrinsic data storage and data processing capabilities to enable data scientists to Good mining and the value of the data.

## Eco-system of Apache Hadoop Submarine Miscs Project

### submarine installer

Hadoop has enabled YARN to support Docker container since 2.x. **Hadoop {Submarine}** then uses YARN to schedule and run the distributed deep learning framework in the form of a Docker container.

Since the distributed deep learning framework needs to run in multiple Docker containers and needs to be able to coordinate the various services running in the container, complete the services of model training and model publishing for distributed machine learning. Involving multiple system engineering problems such as `DNS`, `Docker`, `GPU`, `Network`, `graphics card`, `operating system kernel` modification, etc. It is very difficult and time-consuming to properly deploy the **Hadoop {Submarine}** runtime environment.

We have provided you with the installation tool [submarine installer](submarine-installer) for the hadoop submarine runtime environment.

### zeppelin submarine interpreter

A deep learning algorithm project requires data acquisition, data processing, data cleaning, interactive visual programming adjustment parameters, algorithm testing, algorithm publishing, algorithm job scheduling, offline model training, model online services and many other processes and processes. At present, the excellent interactive visual development platform has two main projects, Zeppelin and jupyter. The jupyter is more refined and the algorithm development process, In addition to machine learning algorithm writing and graphical display data, Zeppelin can also process data processing.

We have developed the zeppelin interpreter for Hadoop submarine. With the zeppelin submarine interpreter, you can directly develop, debug and visualize deep learning algorithms in zeppelin. We are submitting the zeppelin submarine interpreter to the zeppelin community for everyone. Hadoop submarine can be easily used.

Design documentation: https://docs.google.com/document/d/16YN8Kjmxt1Ym3clx5pDnGNXGajUT36hzQxjaik1cP4A/edit#

### Azkaban submarine job

Azkaban is an easy-to-use workflow scheduling service that schedules the workflow of individual notes and individual paragraphs by azkaban scheduling the hadoop submarine note written in zeppelin.

Design documentation: https://docs.google.com/document/d/1elWfqXFIiKV0nDDjO8WjiLbxG-mY64Wd7dQ0nP5cEYs/edit