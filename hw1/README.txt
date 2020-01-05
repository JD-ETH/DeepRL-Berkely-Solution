

run code:

Run the following command for Section 1 (Behavior Cloning):

$ python cs285/scripts/run_hw1_behavior_cloning.py --expert_policy_file cs285/policies/experts/HalfCheetah.pkl --env_name HalfCheetah-v2 --exp_name test_bc_hcheetah --n_iter 1 --expert_data cs285/expert_data/expert_data_HalfCheetah-v2.pkl --batch_size=1000 --eval_batch_size=5000
Run the following command for Section 2 (DAGGER):

$ python cs285/scripts/run_hw1_behavior_cloning.py --expert_policy_file cs285/policies/experts/Humanoid.pkl --env_name Humanoid-v2 --exp_name test_dg_humanoid --n_iter 20 --expert_data cs285/expert_data/expert_data_Humanoid-v2.pkl --video_log_freq 5 --do_dagger --batch_size=1000 --eval_batch_size=5000

Conclusion:

- Half Cheetah is easier to learn by vanilla imitation learning than Humanoid.
- Dagger improves learning behavior by pulling trajectory distribution between training and test closer together.