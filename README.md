Test of the TabNet algo

Good walkthrough by M Huss https://followthedata.wordpress.com/

From PyCharm command line:
run:

python train_tabnet.py --csv-path data/np.csv --target-name "is_NP"  --task classification

modified the train_tabnet.py to calcualte AUC metric
optimize parameters:
python opt_tabnet.py --csv-path data/np.csv --target-name "is_NP"  --task classification

Best parameter setting: {'batch_momentum': 0.874136493427681, 'gamma': 0.5383529492172767, 'lambda': 1, 'n_a': 64.0, 'n_steps': 5.0}
