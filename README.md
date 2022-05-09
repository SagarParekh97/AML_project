# A Comparative Analysis of IMU based Motion Prediction Methods

To explore the effects of the different types of network architectures on the human pose estimation, we implement four
different architectures: (1) Bidirectional LSTM, (2) Unidirectional LSTM, (3) Bidirectional GRU, (4) Unidirectional
GRU. We train models based on these architectures using the DIP-IMU Dataset.


The DIP-IMU dataset can be downloaded from the following link:

Unzip the dataset in the folder /AML_project

The Bidirectional LSTM model can be trained as follows:

```bash
python3 DIP_IMU_NN_BiRNN.py --run-name lstm_bi --network LSTM --bidirectional --train --epochs 30
```
For training the other models, you can use the arguments we provided in `./hyparameters.yaml`.

If you just wish to plot the data obtained from previously trained models, use the following command:

```bash
python3 DIP_IMU_NN_BiRNN.py --run-name <name_of_run_you_wish_to_plot> 
```