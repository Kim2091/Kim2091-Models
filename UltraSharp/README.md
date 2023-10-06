Original Release Info:

**Name:** 4x-UltraSharp

**License:** CC BY-NC-SA 4.0

**Link:** <https://mega.nz/folder/qZRBmaIY#nIG8KyWFcGNTuMX_XNbJ_g>

**Model Architecture:** ESRGAN

**Scale:** 4

**Purpose:** Any, it's universal. This model performs best on JPEG compressed images.

**Iterations:** 150k

**batch_size:** 4-8

**HR_size:** 128

**Epoch:** ~480

**Dataset:** So many. I used: RAW images shot by myself, SignatureEdits, AdobeMIT-5K, DIV2K, and many images provided by @musl (thanks!)

**Dataset_size:** uh, ignore this. anywhere between 2k and 8k full size images throughout training

**OTF Training** Yes (custom augmentation presets)

**Pretrained_Model_G:** 4x-UniScale-Balanced


**Description:** This is my best model yet! It generates lots and lots of detail and leaves a nice texture on images. It works on most images, whether compressed or not. It does work best on JPEG compression though, as that's mostly what it was trained on. It has the ability to restore highly compressed images as well!

The model was trained with KernelGAN (thanks musl for supplying the blur kernels), noise patches, custom augmentation presets (will be linked below), and the losses: pixel, feature, cx, ssim, lpips, and fft. Mixup was used for a while, but abandedoned due to stability issues.

Gradient Clipping helped immensely with model stability throughout training, I highly recommend it.

===== EXTRA INFO =====

The Beta version of the model is from the first go at it. I started over for the released version. That model is really good at deblurring some objects that this one doesn't, but it also causes many many issues (hence the restart). It does work better on DDS/BC compression. Other than that, it doesn't really have many advantages.
