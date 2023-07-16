# safe-control-project-2023

Software:
   We only change the internal structure, the usage is the same as before.
   The details of the changes are as follows:
   Added a new file: `attitude_control.py`
   [attitude_control.py](https://github.com/peilin1011/safe-control-gym/blob/main/safe_control_gym/envs/gym_pybullet_drones/attitude_control.py)
   - Path: `safe-control-gym/safe_control_gym/envs/gym_pybullet_drones/attitude_control.py`
   - This file implements the attitude control part based on the Mellinger controller.
   analog the attitude control part in mellinger controller
   change a file: ‘quadrotor.py’
   [quadrotor.py](https://github.com/peilin1011/safe-control-gym/blob/main/safe_control_gym/envs/gym_pybullet_drones/quadrotor.py)
   - `attitude_control.py` is now imported in `quadrotor.py`.
   - Line 576 - 627: Modified the 3D part (`self.QUAD_TYPE == QuadType.THREE_D`) in the function `_setup_symbolic(self, prior_prop={}, **kwargs)`.
   - Line 815 - 848: Modified the function `_preprocess_control(self, action)`.

