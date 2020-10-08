# MyMLmodel

The pipline config file are the specifications for the ssd ResNet 640*640 model i was using. I followed the tutorial basically step by step, except for the tagging and converting to tfrecords because they were already exported from VoTT as tfrecords. 


This is the tutorial i followed:
https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/training.html

after follwing the steps, i cd'ed into the training demo folder and ran this command in the command prompt:

Training:
"python model_main_tf2.py --model_dir=models/my_ssd_resnet50_v1_fpn --pipeline_config_path=models/my_ssd_resnet50_v1_fpn/pipeline.config"

Evaluation:

"python model_main_tf2.py --model_dir=models/my_ssd_resnet50_v1_fpn --pipeline_config_path=models/my_ssd_resnet50_v1_fpn/pipeline.config --checkpoint_dir=models/my_ssd_resnet50_v1_fpn"

and then for tensorboard i ran:
"Conda Activate TensorFlow"
"tensorboard --logdir=models/my_ssd_resnet50_v1_fpn"

