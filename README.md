# DeepLearningBugsData

## Introduction

This is a dataset created to support paper: **Toward Understanding Deep Learning Framework Bugs**

To fully research the characteristic and distribution of bugs in DL frameworks, we collected closed and merged pull request from four famous DL library repositories: TensorFlow, PyTorch, MXNet and Deeplearning4J. In total we analysed 954 pull requests and collected 800 bugs. All bugs are recorded in the excel table.

## Repository

Four repository links are displayed as follows. 

TensorFlow: https://github.com/tensorflow/tensorflow

PyTorch: https://github.com/pytorch/pytorch

MXNet: https://github.com/apache/incubator-mxnet

Deeplearning4J: https://github.com/eclipse/deeplearning4j

## Information

Here we introduce some important labels in the worksheet.

-issue: issue id solved by or relevant to the pull request.
-pr_id: short for pull request id.
-start_time: time when relevent issue was created.
-merge_time: time when pull request was merged.
-patch_file: files that contributor pulled to solve the issue.
-symptom: the symptom created by bugs.
-root_cause: the root cause of bugs.
-root_cause-sub: records of subcategories in root cause.
-component: the category where the bugs happens in DL framework.
-stage: period when bugs happens.
-function_num: function numbers modified in the pull request.

