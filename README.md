# FFE: Fingerprint Frequency Estimation Benchmark

The Fingerprint Frequency Estimation (FFE) benchmark is the first dedicated resource for evaluating frequency estimation methods. 
It consists of a “Good” dataset with 10 high-quality fingerprints and a “Bad” dataset with 50 low-quality fingerprints. 
For each fingerprint, the benchmark provides the following ground truth data: 
- segmentation mask,
- orientation field,
- frequency map.

By including segmentation and orientation ground truth, the benchmark allows to assess the performance of frequency estimation methods independently of potential biases introduced by other processing steps.

The FFE benchmark has been designed with the following characteristics:
- Dense pixel-wise ground truth – unlike most annotated fingerprint datasets, features are not provided on a sparse grid. Every pixel has its corresponding ground truth data, offering richer information for evaluation.
- Simple and familiar storage format – all data is stored in the widely used Portable Network Graphics (PNG) format. In particular, for each fingerprint, the benchmark contains four grayscale images with one byte per pixel. This simplifies access and integration with existing tools and software libraries.
- Straightforward evaluation metric – The benchmark utilizes the Mean Absolute Percentage Error (MAPE) for easy-to-understand and readily implementable performance assessment.

For more information on this benchmark, including evaluation metric and storage format, please see [1].

## References
[1] (Paper under review)
