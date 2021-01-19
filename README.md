# Generative Adversarial Networks Cheat Sheet

### Table of Contents

### Introduction

#### Generative Models vs. Discriminative Models

| Discriminative Models        | Generative Models                          |
| ---------------------------- | ------------------------------------------ |
| Features $\rightarrow$ Class | Random Noise, Class $\rightarrow$ Features |

#### Generative Models 

| Variational Autoencoders (VAEs)                              | Generative Adversarial Networks (GANs)                       |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Encoder :dog2: $\rightarrow$ Latent Space :world_map: $\rightarrow$ Decoder :poodle: | Random Noise :shit: $\rightarrow$ Generator $\rightarrow$ :dog2: $\longleftrightarrow$ Discriminator |

#### GANs Applications

| StyleGAN2                 | CycleGAN                   | GauGAN          |
| ------------------------- | -------------------------- | --------------- |
| Generate :man::dog2::cat: | Image-to-image translation | Image Synthesis |

| Adobe              | Google          | IBM               | SnapChat      | Disney           |
| ------------------ | --------------- | ----------------- | ------------- | ---------------- |
| Next-gen Photoshop | Text Generation | Data Augmentation | Image Filters | Super-resolution |

#### GANS Intuition

| Generator                           | Discriminator                       |
| ----------------------------------- | ----------------------------------- |
| learns to make fakes that look real | learn to distinguish real from fake |



```flow
st=>start: Noise
gen=>operation: Generator
fea=>operation: Features
dis=>operation: Discriminator
out=>operation: Output
cost=>operation: Cost

st->gen->fea->dis->out->cost->gen
```





