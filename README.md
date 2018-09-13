Weapon detection on image of x-ray scanned baggage


authors: Mateusz Paskuda, Dawid Kubów


To launch project:

1. Install Tensorflow https://www.tensorflow.org/install/
2. In command line type : 
$ pip install "tensorflow>=1.7.0"
$ pip install tensorflow-hub
3. Run command python retrain.py --image_dir .\xray (you can combine with --how_many_training_steps for example: --how_many_training_steps=500 -> default value is 4000, more steps more calculation time) 
4. Run command: python label_image.py --graph=\tmp\output_graph.pb --labels=\tmp\output_labels.txt --input_layer=Pla
ceholder --output_layer=final_result --image=.\B0076_0012.jpg      ( to test)
5. You can run command: tensorboard --logdir \tmp\retrain_logs (to launch tensorboard and open it in internet browser)
