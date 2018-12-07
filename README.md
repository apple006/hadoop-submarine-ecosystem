# hadoop-submarine-ecosystem

Hadoop {Submarine} is the latest machine learning framework subproject in the Hadoop 3.2 release. It allows Hadoop to support `Tensorflow`, `MXNet`,` Caffe`, `Spark`, etc. A variety of deep learning frameworks provide a full-featured system framework for machine learning algorithm development, distributed model training, model management, and model publishing, combined with hadoop's intrinsic data storage and data processing capabilities to enable data scientists to Good mining and the value of the data.

## Eco-system of Hadoop Submarine Project

### submarine installer

Hadoop has enabled YARN to support Docker container since 2.x. **Hadoop {Submarine}** then uses YARN to schedule and run the distributed deep learning framework in the form of a Docker container.

Since the distributed deep learning framework needs to run in multiple Docker containers and needs to be able to coordinate the various services running in the container, complete the services of model training and model publishing for distributed machine learning. Involving multiple system engineering problems such as `DNS`, `Docker`, `GPU`, `Network`, `graphics card`, `operating system kernel` modification, etc. It is very difficult and time-consuming to properly deploy the **Hadoop {Submarine}** runtime environment.

We have provided you with the installation tool [submarine installer](submarine-installer) for the hadoop submarine runtime environment.

### zeppelin submarine interpreter

A deep learning algorithm project requires data acquisition, data processing, data cleaning, interactive visual programming adjustment parameters, algorithm testing, algorithm publishing, algorithm job scheduling, offline model training, model online services and many other processes and processes. At present, the excellent interactive visual development platform has two main projects, Zeppelin and jupyter. The jupyter is more refined and the algorithm development process, In addition to machine learning algorithm writing and graphical display data, Zeppelin can also process data processing.

We have developed the zeppelin interpreter for Hadoop submarine. With the zeppelin submarine interpreter, you can directly develop, debug and visualize deep learning algorithms in zeppelin. We are submitting the zeppelin submarine interpreter to the zeppelin community for everyone. Hadoop submarine can be easily used.

https://docs.google.com/document/d/16YN8Kjmxt1Ym3clx5pDnGNXGajUT36hzQxjaik1cP4A/edit#