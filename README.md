# Phenotype Extraction

This R notebook is written to extract phenotype information from drone imagery.

## Download the GitHub repo

Download the repo by clicking Code > Download ZIP:

![Alt text](img/download_zip.png?raw=true "Title")

Now, extract the contents of the ZIP file:

![Alt text](img/extract_zip.png?raw=true "Title")

Copy the path of the folder:

![Alt text](img/contents_filepath.png?raw=true "Title")

In RStudio, set the working directory to this copied path:

![Alt text](img/set_wd.png?raw=true "Title")

<!-- ![Alt text](img/open_folder.png?raw=true "Title") -->

![Alt text](img/home_dir.png?raw=true "Title")

## Install FieldImageR

We must first install devtools, which allows us to install software from GitHub:

```
install.packages("devtools")
```

![Alt text](img/install_devtools.png?raw=true "Title")

We can now install FieldImageR:

```
devtools::install_github("OpenDroneMap/FIELDimageR")
```

![Alt text](img/install_fieldimageR.png?raw=true "Title")

Confirm the successful installation of FieldImageR by searching for "FIELDimageR" in your Packages section. If you see the package, the installation was successful. Try the installation again if you do not see the package.

![Alt text](img/install_confirm.png?raw=true "Title")

## Run R notebook
<!-- 
Before running the code, we need to download the orthomosaic by [clicking here](https://data.cyverse.org/dav-anon/iplant/projects/phytooracle/season_16_sorghum_yr_2023/level_1/drone/North-Cardon-Lane-7-6-2023-orthophoto.tif). -->

<!-- Make sure that the orthomosaic is in your working directory:

![Alt text](img/ortho_working.png?raw=true "Title") -->

Let's try to run the R notebook named `testing_fieldimageR.Rmd` in the current repo. Click on Run > Run All:

![Alt text](img/run_code.png?raw=true "Title")

By default, RStudio displays figures inline, which creates a problem when trying to run certain FieldImageR functions:

![Alt text](img/error.png?raw=true "Title")

## Direct figures to the console

To fix this, we need to direct figure outputs to the console:

![Alt text](img/fix_error.png?raw=true "Title")

Now, the figures will be directed to the console, and we can now select points:

![Alt text](img/point_selection.png?raw=true "Title")

## Troubleshooting

There are some cases where the mouse cursor locations are offset. This is often due to the scale of your display. 

To fix this in Windows, go to Settings > Display > Scale and change it to 100%. If this is set to anything other than 100%, your mouse cursor locations will be offset.

On my display, the recommended setting is 150%, but this resulted in issues with my cursor locations, so I switched to 100%:

![Alt text](img/scale_setting.png?raw=true "Title")