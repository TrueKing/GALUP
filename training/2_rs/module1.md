# Module 1 - Introduction to Remote Sensing

**What will you learn from this module?**

- Basics of remote sensing (RS), Electromagnetic (EM) spectrum, wavelengths/bands
- Different types of remote sensing systems, sensors, and resolutions
- Sources for remote sensing data

## Definition
**Remote sensing** is the science and art of obtaining information about an object, area, or phenomenon through the analysis of data acquired by a device that is not in contact with the object, area, or phenomenon under investigation<sup>1</sup>. Modern day remote sensing started with the advent of radar, sonar, and thermal infrared detection systems during World War II. Since then, detectors have been expanded to obtain information from most of the bands in the EM spectrum, with a variety of applications spanning from military use to agriculture. 

## 1. Electromagnetic (EM) Spectrum 

- **EM spectrum** is the entire distribution of electromagnetic radiation according to frequency or wavelength. The Figure below shows the different wavelegth regions in the spectrum and the Table highlights the optical, infrared and microwave Regions that are most commonly used in Earth remote sensing. 

:pushpin: Note that the wavelengths increase as we move across Gamma Ray --> Optical/Visible --> Infrared --> Radio Regions of the spectrum. Thus,
   - The radiation observed in **optical and infrared wavelengths (bands)** 
       > is sensitive to molecular resonances **in the surface layer** of target.<br>
       > is obstructed by clouds, carbon dioxide, and water vapor in the atmosphere.<br>
       > is dependent on solar illumination (_optical and near-infrared_).<br>
    
   - The radiation observed in the **microwave bands** 
      > is sensitive to **temperature distribution, geometric, and electric properties of surface and volume**. <br>
      > can penetrate through clouds and light rain. It may also penetrate through vegetation and provide soil information.<br>
      > is independent of solar illumination.<br>

<br>
<p align="center">
 <img width="604" height="207" src="https://user-images.githubusercontent.com/87503837/132062813-8bd2faa0-336c-4fc7-b3f1-f8ae62822e9b.png">
</p>

<div align="center">

 
|         Bands            |     Wavelengths      |
|--------------------------|----------------------|
|   Blue                   |     0.45-0.51µm      |
|   Green                  |     0.53-0.59µm      |
|   Red                    |     0.64-0.67µm      |
|   Near Infrared          |     0.75-1µm         |
|   Short-wave infrared 1  |     1-1.6µm          |
|   Short-wave infrared 2  |     1.6-2.5µm        |
|   Thermal Infrared       |     10.60–12.51µm    |
|   Microwave              |     1mm - 1m         |
 
</div>

- The human eye is only able to detect in optical wavelengthsm while many insects see in the 300 to 650 nm region, and can detect ultraviolet light because   they have special photoreceptors in their eyes.   


## 2. Remote Sensing Systems and Sensors

### 2.1 Satellite Systems <br>
-	**Geo-stationary/geo-synchronous** : follows direction of Earth's rotation and provides regional coverage. E.g. weather satellites <br>
-	**Polar orbiting**: circle the Earth in an almost north-south orbit, passing close to both poles and providing global coverage. E.g. Landsat series <br>
-	**Neither**: the orbit is based upon science requirements. E.g. Megha-Tropiques covers +/- 20 deg. <br>

### 2.2 Types of Sensors: <br>
- **Active Sensors** consists of a transmitter and a receiver that may be co-located (monostatic system) or may be installed on different satellites (bistatic system). It transmits a known signal at a particular wavelength and receives some portion of the signal in the direction of a receiver. In case of a monostatic system, the received signal is called “backscatter.” E.g. camera with the flash (_optical_), Light Detection and Ranging (LIDAR) (_optical/NIR_), Radio Detection and Ranging (RADAR)(_microwave_). <br>
- **Passive Sensor** consists of a receiver that receives naturally occurring EM energy from a target at a particular wavelength and direction. Examples include a camera without the flash (optical) and radiometers.

### 2.3 Types of Resolutions: <br>
- **Spatial resolution** describes how far apart two targets have to be so that they are detected as separate signals.<br>
- **Temporal resolution** describes how often a sensor observes the same target . <br>
- **Radiometric resolution** describes the number of wavelengths observed. For example, in the Figures below, a multispectral sensor observing about 10s of discrete bands and a hyperspectral sensor observing 100s of bands in the optical/NIR region.<br>
 
<br/>

<p align="center"> <b> Spectral sampling: Multispectral sensors (left) and Hyperspectral sensors (right) </b> <p>

<p align="center"> 
<img src="https://user-images.githubusercontent.com/87503837/133636464-24493df3-1c5d-405f-b7ec-10fe64cec5e7.png" width="400" height="220"><img src="https://user-images.githubusercontent.com/87503837/133636485-93336e1a-214b-4897-b1ca-c1206879b4e1.png" width="400" height="220"> 
 </p>

<br/>

<p align="center"> 
  <img src = "https://user-images.githubusercontent.com/87503837/130195843-a8aea0e9-def9-40c4-80ce-b562fd56e918.png"/>
</p> <br/>

## 3. Data Sources
Satellite data can be obtained from multiple sources, some important repositories are:
- <a href="https://earthexplorer.usgs.gov/">USGS Earth Explorer</a>
- <a href="https://search.earthdata.nasa.gov/search?ac=true">NASA Earthdata Search</a>
- <a href="https://worldview.earthdata.nasa.gov/">NASA Worldview</a>
- <a href="https://scihub.copernicus.eu/dhus/#/home">Copernicus Open Access Hub</a>

The USGS has provided an excellent resource for choosing the best Landsat bands based on application domains; see link <a href="https://www.usgs.gov/faqs/what-are-best-landsat-spectral-bands-use-my-research?qt-news_science_products=0#qt-news_science_products">here</a>. In general, data from other satellites (for e.g., Sentinel-2) can be substituted for Landsat when different spatio-temporal characteristics are desired.

The Table below provides bands from the Landsat satellite program, with the differences between Landsat 5, 7, and 8 outlined.

<p align="center">
<img src="https://user-images.githubusercontent.com/84922404/134026792-d1f488cd-3630-4266-ad2f-ed7062e52982.png" width="500" height="600">
</p>

For further information on remote sensing, this [video](https://www.youtube.com/watch?v=qiqUAlJK4vI) from NASA ARSET is a useful resource.

</p> <br/>

## Practice Exercise and Post-Module Survey (required)

1. Download [practice_m1.zip](https://github.com/SERVIR-WA/GALUP/files/7507592/practice_m1.zip) and unzip the file. The file consists of a vegetation index and land surface temperature data from the MODIS sensor.
2. Open a blank project in QGIS and load both TIF files as layers (drag and drop). 
3. Switch between the two layers to see the difference between the two types of remote sensing data. Which file has a higher resolution? 
4. Take screen shots of the two layers displayed in QGIS and add them to the [template](https://github.com/SERVIR-WA/GALUP/files/7493535/WS2_M1E1_Submission.docx). 
5. Submit the final document <a href="https://github.com/SERVIR-WA/GALUP/issues/new?assignees=&labels=exercise+w2m1&template=w2m1-exercise-submission.md&title=Module+1+exercises+%5Breplace+with+your+name%5D" title="here">here</a>\.
6. Submit the Post-Module [survey](https://ufl.qualtrics.com/jfe/form/SV_9ulL78WT64RMm1M). 
##

**Next Section**: 

<a href="module2.md" title="Module 2">Module 2</a>
