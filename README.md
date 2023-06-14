# How to replicate the emotion diary

1. Clone the directory.

2. Open `PPG Emotion Detection Model.ipynb`

   Set `PROJECT_DIR` appropriately.

   If you run it in local, set `COLAB = False`

   Run all the cells. It will make `model.keras` in `MODEL_DIR` . In default, it is {PROJECT_DIR}/Models/. 

   It also prints median, MAD, mean and standard devaiation of training set. Note these values.

3. Open `Arduino Model.ipynb`

   Run the cells in the first heading "Make a TinyML Lite Model for Arduino"

   `model.cc` will saved.

4. Copy the value in model.cc into `ArduinoEmotionDiary/model.cpp`

5. Run `ArduinoEmotionDiary.ino` according to your purpose. To test interaction, define `RUN_BY_USER` in `constants.h` . To test data collection, comment it out.