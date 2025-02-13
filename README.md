boxuser@TRUSSES9:~/ros2_ws$ MAKEFLAGS="-j1" colcon build --parallel-workers 1 --packages-select chrono_sim
Starting >>> chrono_sim
--- stderr: chrono_sim                             
/home/vboxuser/ros2_ws/src/chrono_sim/src/experiments/triangle_sim.cpp: In function ‘int main(int, char**)’:
/home/vboxuser/ros2_ws/src/chrono_sim/src/experiments/triangle_sim.cpp:148:44: error: ‘std::shared_ptr<chrono::ChBody> Truss::m_body’ is private within this context
  148 |     sph0->Initialize(spirit0->m_trusses[0].m_body, spirit1->m_body,
      |                                            ^~~~~~
In file included from /home/vboxuser/ros2_ws/src/chrono_sim/include/sim_tools/Spirit.h:8,
                 from /home/vboxuser/ros2_ws/src/chrono_sim/include/sim_tools/SpiritFactory.h:14,
                 from /home/vboxuser/ros2_ws/src/chrono_sim/src/experiments/triangle_sim.cpp:32:
/home/vboxuser/ros2_ws/src/chrono_sim/include/sim_tools/Truss.h:59:37: note: declared private here
   59 |     std::shared_ptr<chrono::ChBody> m_body;
      |                                     ^~~~~~
/home/vboxuser/ros2_ws/src/chrono_sim/src/experiments/triangle_sim.cpp:153:44: error: ‘std::shared_ptr<chrono::ChBody> Truss::m_body’ is private within this context
  153 |     sph1->Initialize(spirit1->m_trusses[0].m_body, spirit2->m_body,
      |                                            ^~~~~~
In file included from /home/vboxuser/ros2_ws/src/chrono_sim/include/sim_tools/Spirit.h:8,
                 from /home/vboxuser/ros2_ws/src/chrono_sim/include/sim_tools/SpiritFactory.h:14,
                 from /home/vboxuser/ros2_ws/src/chrono_sim/src/experiments/triangle_sim.cpp:32:
/home/vboxuser/ros2_ws/src/chrono_sim/include/sim_tools/Truss.h:59:37: note: declared private here
   59 |     std::shared_ptr<chrono::ChBody> m_body;
      |                                     ^~~~~~
/home/vboxuser/ros2_ws/src/chrono_sim/src/experiments/triangle_sim.cpp:158:44: error: ‘std::shared_ptr<chrono::ChBody> Truss::m_body’ is private within this context
  158 |     sph2->Initialize(spirit2->m_trusses[0].m_body, spirit0->m_body,
      |                                            ^~~~~~
In file included from /home/vboxuser/ros2_ws/src/chrono_sim/include/sim_tools/Spirit.h:8,
                 from /home/vboxuser/ros2_ws/src/chrono_sim/include/sim_tools/SpiritFactory.h:14,
                 from /home/vboxuser/ros2_ws/src/chrono_sim/src/experiments/triangle_sim.cpp:32:
/home/vboxuser/ros2_ws/src/chrono_sim/include/sim_tools/Truss.h:59:37: note: declared private here
   59 |     std::shared_ptr<chrono::ChBody> m_body;
      |                                     ^~~~~~
gmake[2]: *** [CMakeFiles/triangle_sim.dir/build.make:76: CMakeFiles/triangle_sim.dir/src/experiments/triangle_sim.cpp.o] Error 1
gmake[1]: *** [CMakeFiles/Makefile2:949: CMakeFiles/triangle_sim.dir/all] Error 2
gmake: *** [Makefile:146: all] Error 2
---
Failed   <<< chrono_sim [5.63s, exited with code 2]

Summary: 0 packages finished [5.83s]
  1 package failed: chrono_sim
  1 package had stderr output: chrono_sim
