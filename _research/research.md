---
layout: archive
title: "Research and Thesis"
collection: research
author_profile: true
permalink: /research/ 
---

<html>
<hr color="000000" />
</html>
<br/>

# <i>Individual Project</i>
---
## <b>Real-time 3D Path Planning from a Single Fluoroscopic Image for Robot Assisted Fenestrated Endovascular Aortic Repair (FEVAR)</b>
* 2018, _Imperial College London, London, UK_
<h4><a href="javascript:void(0)" class="dsphead" onclick="dsp(this)"><span class="dspchar">+</span> Detail</a></h4>
<div class="dspcont" style='display:none;'>
  <fieldset>
  <ul>
    <li><b>Motivation</b>: To navigate robot-assisted fenestrated endovascular aortic repair.</li>
    <li><b>Pipeline</b>: 
      <ul>
        <li>Segmented Abdominal Aortic Aneurysm (AAA) using U-Net with data augmentation of grey value variation instead of rotation and mirroring to avoid overfitting caused by relatively small intra-subject variation of intensity and translation. </li>
        <li>Extracted the largest connected area from the segmented volume and reconstruct the 3D AAA shape using marching cube. </li>
        <li>Extracted the centrelines of AAA from CTA and fluoroscopy image. </li>
        <li>Establish the correspondence between the 3D preoperative and 2D intra-operative AAA skeletons using a proposed graph matching method. </li>
        <li>Deformed the 3D skeletons using thin plate spline with regularization in respect to skeleton length and smoothness for the non-rigid 2D/3D registration. </li>
        <li>Validated the proposed framework on simulation, phantom and patient AAA data sets, achieving 3D distance error of 2mm in the phantom setup. </li>
        <li>Obtained also performance advantages in terms of accuracy, robustness and time-efficiency.</li>
      </ul>
    </li>
    <li>[<u><a href="https://jianqingzheng.github.io/publication/ICRA2019-3d_zheng">publication1</a></u>],[<u><a href="https://jianqingzheng.github.io/publication/HSMR2018-abdominal_zheng">publication2</a></u>],[<u><a href="https://github.com/jianqingzheng/path_planning_for_FEVAR">code</a></u>]</li>
  </ul>
  <br/>
  <img src='/images/aaaseg2d_2.gif' />
  <img src='/images/aaaseg3d.png' />
  <img src='/images/demo-recover.gif' />
  <img src='/images/demo-visual.gif' />
  </fieldset>
</div>
<hr color="#FFFFFF" />

## <b>Load Frequency Control of a Smart Grid</b>
* 2016, _University of Liverpool, Liverpool, UK_
<h4><a href="javascript:void(0)" class="dsphead" onclick="dsp(this)"><span class="dspchar">+</span> Detail</a></h4>
<div class="dspcont" style='display:none;'>
  <fieldset>
  <ul>
    <li><b>Motivation</b>: To investigate on the potential usage of direct load control in load frequency control of a smart grid.</li>
    <li><b>Pipeline</b>: 
      <ul>
        <li>Built a mathematical model and the simulated one of Load Frequency Control and Direct Load Control in a multi-area power system. </li>
        <li>Decoupled frequency of each area by solving an equivalent optimization problem of minimizing flow network. </li>
        <li>Utilized direct controlled load to improve the efficiency and stability of the power system and validated the results with simulation.</li>
      </ul>
    </li>
  </ul>
  <br/>
  <img src='/images/powersystem.jpg' />
  <img src='/images/frequencydev.jpg' />
  </fieldset>
</div>
<hr color="#FFFFFF" />

## <b>Capacitive Touch Sensing Device</b>
* 2015, _Wuhan University, Wuhan, CN_
<h4><a href="javascript:void(0)" class="dsphead" onclick="dsp(this)"><span class="dspchar">+</span> Detail</a></h4>
<div class="dspcont" style='display:none;'>
  <fieldset>
  <ul>
    <li><b>Motivation</b>: To design and develop a capacitive touch sensing module used in toys.</li>
    <li><b>Pipeline</b>: 
      <ul>
        <li>Designed a printed circuit board and the coniguration of capacitance sensor and the sensing circuit.</li>
        <li>Analyzed electromagnetic coupling. Added an identification wire to each connected signal wire to compensate for current errors caused by the stray capacitances and parasitic capacitances between the connected wires and ground wire. </li>
        <li>Applied logic circuits to filter fake signals triggered by noise.</li>
      </ul>
    </li>
    <li>[<u><a href="https://jianqingzheng.github.io/publication/UMP2016-logic_zheng">patent</a></u>]</li>
  </ul>
  <br/>
  <img src='/images/patent1.png' />
  <img src='/images/patent2.png' />
  </fieldset>
</div>
<hr color="#FFFFFF" />

## <b>Image Mosaic of Unmanned Aerial Vehicle</b>
* 2015, _Xi’an Jiaotong-Liverpool University, Suzhou, CN_
<h4><a href="javascript:void(0)" class="dsphead" onclick="dsp(this)"><span class="dspchar">+</span> Detail</a></h4>
<div class="dspcont" style='display:none;'>
  <fieldset>
  <ul>
    <li><b>Motivation</b>: To implement an automatic program for image mosaic for a unmanned aerial vehicle.</li>
    <li><b>Pipeline</b>: 
      <ul>
        <li>Implemented noise reduction using a Wiener filter. Utilized the random sample consensus algorithm for image registration based on feature points extracted by the Scale-Invariant Feature Transform in MATLAB.</li>
        <li>Applied weighted averaging to image fusion. </li>
        <li>Completed a MATLAB program that implemented an automatic image mosaic for given photos.</li>
      </ul>
    </li>
  </ul>
  <br/>
  </fieldset>
</div>

---

<br />

# <i>Collaborated Project</i>
---
## <b>High-resolution Feature Map Propagation in Deep Convolutional Neural Network</b>
* 2018, _Imperial College London, London, UK_
<h4><a href="javascript:void(0)" class="dsphead" onclick="dsp(this)"><span class="dspchar">+</span> Detail</a></h4>
<div class="dspcont" style='display:none;'>
  <fieldset>
  <ul>
    <li><b>Motivation</b>: To investigate on the effect of atrous rate on receptive field in a deep convolutional neural network and to improve the resolution of feature maps and the efficiency of the network.</li>
    <li><b>Pipeline</b>: 
      <ul>
        <li>Theoretically analysed the receptive field (RF) with dilated (atrous) rate setting and the truncation effect.</li>
        <li>Obtained and proved a general solution of atrous rate setting for a uniform distributed RF while large and fully covered RF guaranteed.  </li>
        <li>Proposed a novel network, Atrous Convolutional Neural Network (ACNN) with skip connections and multi-scale consideration as an example for semantic segmentation.  </li>
        <li>Validated ACNN on three bio-medical datasets with high-resolution feature map propagation and reasonable segmentation results, reducing the number of variables by 99.75%, and achieving a reasonable DSC of 0.6~0.7. </li>
      </ul>
    </li>
    <li><b>Contribution</b>: 
      <ul>
        <li>Theoretical analysed and simulated the effect of atrous rate on the receptive field, and the truncation effect. </li>
        <li>Processed data and evaluated segmentation results. </li>
      </ul>
    </li>
  </ul>
  <br/>
  <img src='/images/125.gif' />
  <img src='/images/139.gif' />
  </fieldset>
</div>
<hr color="#FFFFFF" />

## Estimation of Tissue Oxygen Saturation from RGB Images
* 2018, _Imperial College London, London, UK_
<h4><a href="javascript:void(0)" class="dsphead" onclick="dsp(this)"><span class="dspchar">+</span> Detail</a></h4>
<div class="dspcont" style='display:none;'>
  <fieldset>
  <ul>
    <li><b>Motivation</b>: To estimate tissue oxygen saturation directly from RGB images without hyperspectral images for a seamless integration of the proposed method into surgical and diagnostic workflows with standard endoscope systems.</li>
    <li><b>Pipeline</b>: 
      <ul>
        <li>Simulated RGB images and calculated the oxygen saturation from given hyperspectral images.</li>
        <li>Augmented data by flipping and cropping with a slide-window. </li>
        <li>Fed the simulated RGB images and the calculated oxygen saturation to train a conditional Generative Adversarial Network (cGAN).</li>
        <li>Estimated tissue oxygen using pixel-level image-to-image translation by cGAN.</li>
        <li>Evaluated prediction results using with different batch size and weight coefficient.</li>
      </ul>
    </li>
    <li><b>Contribution</b>: 
      <ul>
        <li>Programed data processing.</li>
        <li>Programed data augmentation.</li>
        <li>Trained U-Net as the generator, and CNN as the discriminator.</li>
      </ul>
    </li>
    <li>[<u><a href="https://jianqingzheng.github.io/publication/HSMR2018-estimation_li">publication</a></u>]</li>
  </ul>
  <br/>
  <img src='/images/estimation_method.png' />
  <img src='/images/estimation_result.png' />
  </fieldset>
</div>
<hr color="#FFFFFF" />

## <b>Brain-Computer Interface Framework for NAO Robot</b>
* 2017, _Imperial College London, London, UK_
<h4><a href="javascript:void(0)" class="dsphead" onclick="dsp(this)"><span class="dspchar">+</span> Detail</a></h4>
<div class="dspcont" style='display:none;'>
  <fieldset>
  <ul>
    <li><b>Motivation</b>: To build a brain-computer interface network with electroencephalograph signals for robot control.</li>
    <li><b>Pipeline</b>: 
      <ul>
        <li>Removed the artefacts caused by electromyography and electrooculography from electroencephalograph (EEG) signals using Wavelet Analysis.</li>
        <li>Extracted the features of the EEG signals using Common Spatial Pattern (CSP) filter. Used Linear Discriminant Analysis (LDA), Support Vector Machine (SVM), Convolutional Neural Network (CNN) and Recurrent Neural Network (RNN) to classified two kinds of imaginary motion. </li>
        <li>Transmitted classified data to the second computer with SSH protocol by Python-Socket for real-time control of one NAO robot.</li>
        <li>Implemented colourized boundary distance measurement using histogram equalization to enhance contrast, a Laplacian filter to detect edge and a homogeneous transformation to reconstruct the 3-D coordinates.</li>
        <li>Controlled a NAO robot to walk out of a maze with EEG.</li>
      </ul>
    </li>
    <li><b>Contribution</b>: 
      <ul>
        <li>Optimized the algorithm of artefact removal.</li>
        <li>Extracted feature using CSP filter.</li>
        <li>Classified EEG signal using LDA in MATLAB and OpenVibe as well as kernel SVM in OpenVibe.</li>
        <li>Transmitted classified data with SSH. </li>
      </ul>
    </li>
    <li>[<u><a href="https://jianqingzheng.github.io/publication/UK-RAS2017-motor_zhang">publication</a></u>]</li>
  </ul>
  <br/>
  <img src='/images/eeg_control.jpg' />
  <img src='/images/maze_navig.jpg' />
  </fieldset>
</div>
<hr color="#FFFFFF" />

## <b>Smartphone Download-Management System</b>
* 2016, _University of Liverpool, Liverpool, UK_
<h4><a href="javascript:void(0)" class="dsphead" onclick="dsp(this)"><span class="dspchar">+</span> Detail</a></h4>
<div class="dspcont" style='display:none;'>
  <fieldset>
  <ul>
    <li><b>Motivation</b>: To investigate on management strategies of file downloading in a smartphone.</li>
    <li><b>Pipeline</b>: 
      <ul>
        <li>Built a model of Wi-Fi and 3G data transmissions using MATLAB.</li>
        <li>Simulated a process of file generation and downloads to optimize the downloading process.</li>
        <li>Designed strategies for priority ranking, and optimized loss functions.</li>
        <li>Implemented the data dynamic visualization of download values and download size for different strategies.</li>
        <li> Quantified the performance of each strategy according to the size and value of downloaded documents, tested the simulation in multiple internet environments, and selected the optimal strategies for most cases.</li>
      </ul>
    </li>
    <li><b>Contribution</b>: 
      <ul>
        <li>Leaded the group.</li>
        <li>Designed the framework and downloading strategies.</li>
        <li>Implemented the file generation and data visualization.</li>
      </ul>
    </li>
  </ul>
  <br/>
  <img src='/images/sim_map.png' />
  <img src='/images/download_doc.png' />
  </fieldset>
</div>
<hr color="#FFFFFF" /> 

## Big Data Challenge, Interdisciplinary Contest in Modeling, COMAP
* 2015, _Xi’an Jiaotong-Liverpool University, Suzhou, CN_
<h4><a href="javascript:void(0)" class="dsphead" onclick="dsp(this)"><span class="dspchar">+</span> Detail</a></h4>
<div class="dspcont" style='display:none;'>
  <fieldset>
  <ul>
    <li><b>Motivation</b>: To quantify and optimize the investment strategies to universities with a large dataset.</li>
    <li><b>Pipeline</b>: 
      <ul>
        <li>Replaced outlier and missing data using linear interpolation and averaging.</li>
        <li>Reduced the dimensions of the feature space with principal component analysis.</li>
        <li>Fitted a characteristic curve of investment and performance indexes weighted according to the result of the PCA using a Back-Propagation Neural Network (BP-NN).</li>
        <li>Utilized the Stochastic Gradient Descent method to minimize the cost function based on the Euclidean distance with various, random initial points.</li>
      </ul>
    </li>
    <li><b>Contribution</b>: 
      <ul>
        <li>Programed data pre-processing including normalization, data cleaning, as well as dimension reduction.</li>
        <li>Implemented BP-NN and optimization using MATLAB toolbox.</li>
      </ul>
    </li>
  </ul>
  <br/>
  </fieldset>
</div>
---
