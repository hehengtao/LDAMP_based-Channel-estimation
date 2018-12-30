This code is for the following paper: 

H. He, C. Wen, S. Jin, and G. Y. Li, “Deep learning-based channel estimation for beamspace mmwave massive MIMO
systems,” IEEE Wireless Commun. Lett., vol. 7, no. 5, pp. 852–855, Oct. 2018.


Please cite the paper when use this code.

1. Install Matcovnet 

    Choose the gpu version and verify you have a supported GPU and that the latest driver is installed.

    
2. Run main program 

Location: ..\LDAMP_for_Rice\D-AMP_Toolbox-master\SCAMPI-MATLAB\scampi-vs-ssd\

main_new_old.m: main function, run and call trained network and denoiser to produce simulation results 

test.m: Generate the Saleh-Valenzuela channel model

Trained network is saved at ..\Code_WCL_2018\LDAMP_for_Rice\D-AMP_Toolbox-master\Packages\DnCNN\BestNets_20

3. Trainin DnCNN network

Location: ..\LDAMP_for_Rice\D-AMP_Toolbox-master\Packages\DnCNN\Training

Demo_Train.m: main function for training the DnCNN

Demo_test: main fuction for test the DnCNN

Training_h.mat: Training data

Vali_h.mat: Validata and Test data

rescaleImage.m: rescale the channel into [0,1]

channel_gen.m: generate the training and test data

Many trained network will be saved at ..\LDAMP_for_Rice\D-AMP_Toolbox-master\Packages\DnCNN\Training\NewNetworks. Copy the best network with different SNR and rename to 
..\LDAMP_for_Rice\D-AMP_Toolbox-master\Packages\DnCNN\BestNets_20.

4. LDAMP network

Location: ..\LDAMP_for_Rice\D-AMP_Toolbox-master\SCAMPI-MATLAB and ..\LDAMP_for_Rice\D-AMP_Toolbox-master\Algorithms

DAMP_SNR1.m: D-AMP algorithma

Acknoledge:

Many thanks for Dr.Christopher A. Metzler share the code selflessly. Instructions about installing the matcovnet and using LDAMP network can refer to

website: https://github.com/ricedsp/D-AMP_Toolbox

Questions/suggestions/comments about LDAMP-based Channel estimation network: hehengtao@seu.edu.cn
