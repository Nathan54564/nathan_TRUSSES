# nathan_TRUSSES


Starting >>> chrono_sim
--- stderr: chrono_sim                             
/home/vboxuser/ros2_ws/src/chrono_sim/src/experiments/triangle_sim.cpp: In function ‘int main(int, char**)’:
/home/vboxuser/ros2_ws/src/chrono_sim/src/experiments/triangle_sim.cpp:147:14: error: ‘class Spirit’ has no member named ‘AttachTrussSpherical’
  147 |     spirit0->AttachTrussSpherical(0, spirit1->m_body, ChVector3d(-0.25, 0, 0.025));
      |              ^~~~~~~~~~~~~~~~~~~~
/home/vboxuser/ros2_ws/src/chrono_sim/src/experiments/triangle_sim.cpp:148:14: error: ‘class Spirit’ has no member named ‘AttachTrussSpherical’
  148 |     spirit1->AttachTrussSpherical(0, spirit2->m_body, ChVector3d(-0.25, 0, 0.025));
      |              ^~~~~~~~~~~~~~~~~~~~
/home/vboxuser/ros2_ws/src/chrono_sim/src/experiments/triangle_sim.cpp:149:14: error: ‘class Spirit’ has no member named ‘AttachTrussSpherical’
  149 |     spirit2->AttachTrussSpherical(0, spirit0->m_body, ChVector3d(-0.25, 0, 0.025));
      |              ^~~~~~~~~~~~~~~~~~~~
gmake[2]: *** [CMakeFiles/triangle_sim.dir/build.make:76: CMakeFiles/triangle_sim.dir/src/experiments/triangle_sim.cpp.o] Error 1
gmake[1]: *** [CMakeFiles/Makefile2:949: CMakeFiles/triangle_sim.dir/all] Error 2
gmake: *** [Makefile:146: all] Error 2
---
Failed   <<< chrono_sim [6.28s, exited with code 2]

Summary: 0 packages finished [6.45s]
  1 package failed: chrono_sim
  1 package had stderr output: chrono_sim
