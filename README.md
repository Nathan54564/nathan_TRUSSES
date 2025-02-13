home/vboxuser/ros2_ws/src/chrono_sim/src/experiments/triangle_sim.cpp: In function ‘int main(int, char**)’:
/home/vboxuser/ros2_ws/src/chrono_sim/src/experiments/triangle_sim.cpp:148:44: error: ‘__gnu_cxx::__alloc_traits<std::allocator<Truss>, Truss>::value_type’ {aka ‘class Truss’} has no member named ‘GetConnector’
  148 |     sph0->Initialize(spirit0->m_trusses[0].GetConnector(), spirit1->m_body,
      |                                            ^~~~~~~~~~~~
/home/vboxuser/ros2_ws/src/chrono_sim/src/experiments/triangle_sim.cpp:153:44: error: ‘__gnu_cxx::__alloc_traits<std::allocator<Truss>, Truss>::value_type’ {aka ‘class Truss’} has no member named ‘GetConnector’
  153 |     sph1->Initialize(spirit1->m_trusses[0].GetConnector(), spirit2->m_body,
      |                                            ^~~~~~~~~~~~
/home/vboxuser/ros2_ws/src/chrono_sim/src/experiments/triangle_sim.cpp:158:44: error: ‘__gnu_cxx::__alloc_traits<std::allocator<Truss>, Truss>::value_type’ {aka ‘class Truss’} has no member named ‘GetConnector’
  158 |     sph2->Initialize(spirit2->m_trusses[0].GetConnector(), spirit0->m_body,
      |                                            ^~~~~~~~~~~~
gmake[2]: *** [CMakeFiles/triangle_sim.dir/build.make:76: CMakeFiles/triangle_sim.dir/src/experiments/triangle_sim.cpp.o] Error 1
gmake[1]: *** [CMakeFiles/Makefile2:949: CMakeFiles/triangle_sim.dir/all] Error 2
gmake: *** [Makefile:146: all] Error 2
---
Failed   <<< chrono_sim [5.17s, exited with code 2]

Summary: 0 packages finished [5.34s]
  1 package failed: chrono_sim
  1 package had stderr output: chrono_sim

