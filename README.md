# LINEAR-DISTRIBUTION-FOR-DEEPCACHE
This is a course project exploring non-uniform caching strategies for accelerating diffusion model inference. The original DeepCache uses a fixed uniform interval to schedule full U-Net evaluations during the denoising process. In this project, we challenge that uniformity assumption and propose a Linear Distribution Cache that places full steps according to an arithmetic progression of gaps — front-dense and back-sparse — without changing the total compute budget.

We show that this simple deterministic schedule significantly improves reconstruction fidelity (PSNR, CLIP image similarity) over uniform DeepCache, at identical wall-clock cost, while preserving prompt alignment (CLIP score).

The complete dataset is too large to host on GitHub. Therefore, we only provide the experimental subset (prompts_LITTLE1.csv) used for all reported results. The original full dataset is available at:(https://www.kaggle.com/datasets/tanreinama/900k-diffusion-prompts-dataset/data)
