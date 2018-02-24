The developed models
====================

_The models will be more complex at the end of list_

1. man_pathfind_4j_ik_ompl - a model of manipulation robot: has 7 joints, IK, calculation trajectory to 4 points, use OMPL with debug messages, avoidance of obstacles -- **works, but not every time**
2. frame_gui - a model of frame robot: 5 joints, has custom GUI for control of a joints position, has defined the limits of joints, has target and tip dummy -- **works**
3. frame_gui_convexhull - a model of frame robot: 5 joints, custom GUI, all parts of robot has been included in convex hull -- **works**
4. frame_ik_followPath - a model of frame robot: 5 joints, IK, find a tip configuration (with simGetConfigForTipPose) and follow to it (simGenerateIkPath), the destination is near to the current position -- **works**
5. frame_ik_ompl - a model of frame robot: 5 joints, IK, calculation trajectory with OMPL -- **doesn't work**
6. man_5j_ik_dls - a model of manipulation robot: 5 joints, IK: DLS, manual moving of a target point and following it -- **works**
7. man_pathfind_6j_ik_ompl - a model of manipulation robot: 6 joints, IK, calculation trajectory with OMPL to 4 points except collisions, add a camera to the tip, add joint graphs -- **works**
8. man_pathfind_6j_ik_velocity - a model of manipulation robot: man_pathfind_6j_ik_ompl + speed graphs -- **works**
9. man_6j_opacity - a model of manipulation robot: 6 joints, all element of a robot is transparent (can view joints) -- **works**
10. frame_gui_opacity - a model of frame robot: 5 joints, GUI, all element of a robot is transparent (can view joints) -- **works**
11. frame_max_tests - a model of frame robot: 5 joints, GUI, IK, code: OMPL + Refflex + simGenerateIkPath, PointCloud (to show the limits of work area), elements of a robot in a covex hull, collision detect mode on, add Venera (the detail that will been scaned) - convex hull, add graph of a speed and acceleration -- **works**
12. man_6j_gui_convex - a model of manipulation robot: 6 joints, GUI with degrees, elements of a robot in a covex hull, collision detect mode on -- **works**
13. man_pathfind_6j_ik_ompl_plane - a model of manipulation robot: man_pathfind_6j_ik_ompl + add graphs of degrees of joints, add model of a part of a plane -- **works**
14. man_and_frame__testFrame_bigJoints_proximity - a model of manipulation and frame robot; man: 6 joints, IK (defined but not used); frame: 5 joints, IK, code: simGetConfigForTipPose+simGenerateIkPath, Venera -- **works**
15. man_and_frame__testFrame_reflex_pathAroundVenera -  a model of manipulation and frame robot and Venera: man_and_frame__frame_tests_bigJoints_proximity + calculate path round Venera: simRMLMoveToPosition -- **doesn't work**
16. man_and_frame__gui - all models with GUI, incorrect collections to process collisions -- **works**
17. man_and_frame__testTableRotate - all models, add tests to rotate table on mouse click actions -- **doesn't work**
18. man_and_frame__gui_rotateCamera - all models, rotating camera, GUI on some actions, proximity sensors to visualize x-ray, connected IK manipulator and frame -- **works**
19. man_and_frame__gui_rotateCamera_plane - all models,  rotating camera, GUI, add the part of plane -- **doesn't work**
20. man_and_frame__gui_rotateCamera_plane_path - all models, moving to the path -- **doesn't work**
21. man_and_frame__gui_convex  - all models: manipulator with 6 joints and frame with 5 ones, GUI, convex hulls, collections, visualing a collisions -- **works**