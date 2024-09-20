---
layout: page
title: ET & IT neuron modelling
description: Building a computational model of cortical ET and IT pyramidal neurons during learning of a stimulus-reward association task.
img: assets/img/icon_ET_IT_diagram.png
importance: 2
category: Ongoing
---

Here, I provide a brief overview of my role in this project. We are currently preparing a manuscript for submission to a journal, so I hope I will soon be able to share more information about this exciting project.

<b> Overview </b>

In this project, I collaborated with experimental neuroscientists to build a computational model of layer 5 (pyramidal) ET and IT neurons in a reward association task. 
My role required designing a computational model that could predict the (mice) experimental data.
Since the experimental data involved a stimulus-reward association task, we modelled the value encoding process of the task based on a reinforcement learning update rule.
We used this update rule to train a (linear) neural network to predict the value of several input stimuli. 
We refer to this network as the 'value-encoding' network.
Next, we combined the value-encoding network with a separate convolutional or feedforward auto-encoder model.
The role of this auto-encoder model was to extract useful latent features, which may help the value-encoding network predict the correct value of each input stimulus.
A simplified diagram of the overall model is provided below,
 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ET_IT_diagram.png" title="example image" class="img-fluid rounded z-depth-1"  width="700" height="400" %}
    </div>
</div>
<div class="caption">
    Simplified diagram of the designed IT-ET computational model.
</div>

In this diagram, the IT neurons component corresponds to the encoder block of the auto-encoder model. The auto-encoder was pre-trained on a more general stimulus reconstruction task. An example of the auto-encoder process can be found below,

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/IT_AE.png" title="example image" class="img-fluid rounded z-depth-1" width="500" height="100" %}
    </div>
</div>
<div class="caption">
    Example diagram of the auto-encoder architecture used to pre-train the (IT) encoder block.
</div>

For mice, the stimuli consisted of different whisker stimulation frequencies. In the model, we reproduced the wisker stimulation by generating synthetic data. 

Overall, the model successfully reproduces the experimental data and makes potentially novel predictions about how representational overlap in IT neurons influences the learning of stimulus-reward associations (more on this coming soon).

