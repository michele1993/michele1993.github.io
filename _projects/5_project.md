---
layout: page
title: ET & IT neuron modelling
description: Building a computational model of cortical ET and IT pyramidal neurons during learning of a stimulus-reward association task.
img: assets/img/icon_ET_IT_diagram.png
importance: 2
category: Ongoing
---

Here, I provide a very brief overview of my role in this project. At the moment, we are preparing a manuscript for submission to a journal, so I hope I will soon be able to share way more about this exciting project.

<b> Overview </b>

In this project I collaborated with experimental neuroscientists to build a computational model of layer 5 (pyramidal) ET and IT neurons during learning of a reward association task in mice.
My role requiried designing a computational model that could predict the experimental data.
Since the experimental data was based on a stimulus-reward association task, we modeled the value encoding process of the task based on reinforcement learning update rule.
This update rule was used to train a (linear) neural network to predict the value of several inputs/stimuli. 
We refer to this network as the 'value-encoding' network.
The value-encoding network was combined with a separate convolutional or feedforward auto-encoder model.
The role of this auto-encoder model was to extract useful latent features, which may help the value-predicting network predict the correct value of each stimulus.
A simplfied diagram of the overall model is provided below,
 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ET_IT_diagram.png" title="example image" class="img-fluid rounded z-depth-1"  width="700" height="400" %}
    </div>
</div>
<div class="caption">
    Simplified diagram of the designed IT-ET computational model.
</div>

In this diagram, the IT cell component corresponds to the encoder block of the auto-encoder model. The auto-encoder was pre-trained on a more general stimulus reconstruction task. An example of the auto-encoder process can be found below,

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/IT_AE.png" title="example image" class="img-fluid rounded z-depth-1" width="500" height="100" %}
    </div>
</div>
<div class="caption">
    Example diagram of the auto-encoder architecture used to pre-train the (IT) encoder block.
</div>

In mice the stimuli consisted of different whisker stimulation frequency. In the model, we modelled these by generating some synthetic data. 

