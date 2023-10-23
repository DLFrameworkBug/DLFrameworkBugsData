# DeepLearningBugsData

## Introduction

This repo contains a dataset for supporting the paper: **Toward Understanding Deep Learning Framework Bugs**, which has been accepted by TOSEM 2023.

To fully research the characteristic and distribution of bugs in DL frameworks, we collected closed and merged pull request from four famous DL library repositories: TensorFlow, PyTorch, MXNet and Deeplearning4J. In total we analyzed1,250 pull requests and collected 1000 real bugs, including 250 latest bugs for each DL frameworks. . All bugs are recorded in the `dataset.xlsx` file.

## Repository

Four repository links are displayed as follows. 

TensorFlow: https://github.com/tensorflow/tensorflow

PyTorch: https://github.com/pytorch/pytorch

MXNet: https://github.com/apache/incubator-mxnet

Deeplearning4J: https://github.com/eclipse/deeplearning4j

## Information

Here we introduce some important labels in the worksheet.

- issue: issue id solved by or relevant to the pull request.
- pr_id: short for pull request id.
- start_time: time when relevent issue was created.
- merge_time: time when pull request was merged.
- patch_file: files that contributor pulled to solve the issue.
- symptom: the symptom created by bugs.
- root_cause: the root cause of bugs.
- root_cause-sub: records of subcategories in root cause.
- component: the category where the bugs happens in DL framework.
- stage: period when bugs happens.
- function_num: function numbers modified in the pull request.

## Preliminary application

Guided by our study findings, we conduct a preliminary test case generating tool and deploy it in four versions of TensorFlow. The tool has detected 6 bugs, involving 3 historical bugs and 3 unknown bugs. Regarding 3 unknown bugs, we present the following issue url.

1. Triggered by muate_shape: https://github.com/tensorflow/tensorflow/issues/55214
2. Triggered by mutate_para: https://github.com/tensorflow/tensorflow/issues/55201
3. Triggered by mutate_type: https://github.com/tensorflow/tensorflow/issues/55285
