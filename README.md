# Understanding body planes through MRIs and ItkSnap

The objectives of this homework are:
1. Get familiar with the software [ItkSnap](http://www.itksnap.org) and [3D Slicer](https://www.slicer.org/).
2. Understand the three body planes (Transverse, Sagittal, and Coronal)
3. Introduce the student to the [Itk](https://itk.org/) library and the basic IO functionality. 
4. Continue practicing with [Jupyter Widgets](https://ipywidgets.readthedocs.io/en/stable/).

## Body planes and ItsSnap/3D Slicer (10 Pts)

Using [this T1-weighted MRI brain image](https://drive.google.com/file/d/1bds7Odk_Ugh-Ygc1L0grxEyKFh7xLe2U/view?usp=share_link)
try to identify the following regions in the brain:
* From a Sagittal view:
  * Cerebellum
  * Medulla Oblongata
  * Corpus Callosum
* From a Coronal view:
  * Optic nerve
  * Sylvian fissure
* From a Transverse (Trans) view:
  * Lateral ventricle
  * Caudate nucleus

Google the regions of the brain to find out more information:

![Brain regions](https://www.news-medical.net/image.axd?picture=2020%2F10%2Fshutterstock_284175866.jpg)

For each case make a screenshot of the identified region using the proper plane view and mark the region with an
image-editing software like Photoshop, [Gimp](https://www.gimp.org/), Paint, or even Powerpoint. 

This is an example image showing the *Pons* area from a Sagittal view:

![Pons](https://raw.githubusercontent.com/olmozavala/ds_health_assignment_itksnap/main/Putamen.png)

## Itk and IpWidgets (10 Pts)

Install the Itk library with one of the follwing commands in your python environment:
```shell
pip install itk
conda install -c conda-forge itk
```

Using the `Prostate.mha` file inside the `TestData` folder as an example,
create an IpWidget that displays a view of the 3 planes (similar to ItkSnap) and allows
the user to select the location of each plane with an [IntSlider](https://ipywidgets.readthedocs.io/en/7.6.2/examples/Widget%20List.html#IntSlider).

Similar to the image bellow:
