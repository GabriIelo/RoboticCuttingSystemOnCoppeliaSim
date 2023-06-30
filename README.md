# RoboticCuttingSystemOnCoppeliaSim
The purpose of this project is to create a sort of assembly line suitable for engraving cuboids which will subsequently be moved to a base using a pick and place function.

The IRB140[0] manipulator moves in inverse kinematics following a circular path; a felt pen was used as the end-effector.

The IRB140[1] manipulator moves both in forward and inverse kinematics, in order to make the pick and place work better. The manipulator follows the same trajectory three times; every time a cuboid is placed on the table, the IRB140[1] manipulator waits for a pre-set time to come back into operation, so that the IRB140[0] manipulator completes its routine and frees up the workspace. The script of this manipulator has been taken from a predefined scene of CoppeliaSim and suitably modified for our needs (File/Open scene/ur5WithRg2Grasping).
