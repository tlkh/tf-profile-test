# tf-profile-test

Code at the end of the Jupyter notebook allows you to generate output to see distribution of time spent in various types of compute kernels. Uses TensorFlow 2.0 and requires CUPTI to be installed.

**ResNet 50, XLA + AMP**

```
= type (num_type) % time =
- hmma ( 21 )	 18.9
- fp16 ( 0 )	 0.0
- sgemm ( 3 )	 0.3
- xla ( 868 )	 80.7
Total time: 1066584000000
```

**BERT, XLA + AMP**

```
= type (num_type) % time =
- hmma ( 11 )	 29.9
- fp16 ( 3 )	 0.2
- sgemm ( 3 )	 8.9
- xla ( 593 )	 61.0
Total time: 517483000000

```
