# Steps

- pip install chattts
- Run scripts from chaTTTS.ipynb (Install dependencies if alerted)

- Switch python venv/conda env
- pip install coqui-tts
- Run scripts from coqui.ipynb (Install dependencies if alerted)


- Switch python venv/conda env
- git clone https://github.com/OpenTalker/SadTalker.git
- cd SadTalker || pip install -r requirements.txt
- Download weights from https://drive.google.com/file/d/1gwWh45pF7aelNP_P78uDJL8Sycep-K7j/view
- Extract the weigts file and save in Sadtalker directory (working directory) eg- SadTalker/checkpoints
- Run the following command
  python inference.py --driven_audio <sample-audio-file-path> \
                    --source_image <sample-image-file-path> \
                    --enhancer gfpgan \
                    --checkpoint_dir <checkpoints-dir>
  Example : 
  - python inference.py --driven_audio ../coqui-tts/merged-Michael.wav \
                    --source_image ../image.png \
                    --enhancer gfpgan \
                    --checkpoint_dir ./checkpoints 

