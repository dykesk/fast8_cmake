
generate_f90types(Registry_BeamDyn.txt BeamDyn_Types.f90)

add_library(beamdyn  BeamDyn.f90 BeamDyn_IO.f90 BeamDyn_Subs.f90
  BeamDyn_Types.f90)

target_link_libraries(beamdyn nwtclibs)
