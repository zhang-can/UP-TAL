# Unsupervised Pre-training for Temporal Action Localization (UP-TAL)

PyTorch Implementation of paper:

> **Unsupervised Pre-training for Temporal Action Localization Tasks (CVPR2022)**
>
> Can Zhang, Tianyu Yang, Junwu Weng, Meng Cao, Jue Wang and Yuexian Zou\*.


## Updates

* We will release our codes and models soon, please stay tuned!

## Highlights

* This is the FIRST work focusing on **Unsupervised Pre-training for Temporal Action Localization (UP-TAL)**.

* We design an intuitive and effective pretext task customized for TAL, called **Pseudo Action Localization (PAL)**.

* Our PAL features transfer well on various TAL tasks: Temporal Action Detection (TAD), Action Proposal Generation (APG) and Video Grounding (VG).

## TLDR

<p align="center">
  <img src="https://user-images.githubusercontent.com/32992487/157442511-8de055b0-3892-4885-a74e-9701488726a9.jpg" width="600px" />
</p>

Given a video (<img src="https://render.githubusercontent.com/render/math?math=\boldsymbol{v}_i">), we randomly sample two pseudo action regions from it and then paste them onto another two pseudo background videos (<img src="https://render.githubusercontent.com/render/math?math=\boldsymbol{v}_n"> & <img src="https://render.githubusercontent.com/render/math?math=\boldsymbol{v}_m">) at various temporal locations and scales. PAL learns temporal equivariant features by aligning pseudo action region features (<img src="https://render.githubusercontent.com/render/math?math=\boldsymbol{r}_q"> & <img src="https://render.githubusercontent.com/render/math?math=\boldsymbol{r}_{k%2B}">) and maximizing the agreement between region features of the same video but with different backgrounds.

## Other Info

### Citation

Please **[★star]** this repo and **[cite]** the following paper if you feel our PAL useful to your research:

```
@inproceedings{zhang2022pal,
    title     = {Unsupervised Pre-training for Temporal Action Localization Tasks},
    author    = {Zhang, Can and Yang, Tianyu and Weng, Junwu and Cao, Meng and Wang, Jue and Zou, Yuexian},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    year      = {2022}
}
```

### Contact

For any questions, please feel free to open an issue or contact:

```
Can Zhang: zhang.can.pku@gmail.com
```
